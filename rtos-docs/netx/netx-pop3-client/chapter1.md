---
title: Bölüm 1-Azure RTOS NetX POP3 Istemcisine giriş
description: Azure RTOS NetX POP3 Istemcisi API 'SI, küçük iş istasyonlarının Istemci postasını almak için POP3 sunucularındaki Istemci mailkkkına erişmesi için bir posta aktarım sistemi sağlar.
author: philmea
ms.author: philmea
ms.date: 06/04/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 6abaa778da6203d0df367894165cb29ca629ab5e24403a35af1995f032cf0d4c
ms.sourcegitcommit: 93d716cf7e3d735b18246d659ec9ec7f82c336de
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/07/2021
ms.locfileid: "116798818"
---
# <a name="chapter-1---introduction-to-azure-rtos-netx-pop3-client"></a>Bölüm 1-Azure RTOS NetX POP3 Istemcisine giriş

Post Office protokol sürümü 3 (POP3), küçük iş istasyonlarının istemci postasını almak için POP3 sunucularındaki istemci mailtirmelere erişmesi için posta aktarım sistemi sağlamak üzere tasarlanmış bir protokoldür. POP3, posta aktarımı gerçekleştirmek için Iletim Denetim Protokolü (TCP) hizmetlerini kullanır. Bu nedenle, POP3 son derece güvenilir bir içerik aktarım protokolüdür.

Ancak POP3, posta işleme konusunda kapsamlı işlemler sağlamaz. Genellikle, posta Istemci tarafından indirilir ve ardından sunucunun maildrop 'dan silinir.

## <a name="netx-pop3-client-requirements"></a>NetX POP3 Istemci gereksinimleri

### <a name="client-requirements"></a>İstemci gereksinimleri

Azure RTOS NetX POP3 Istemcisi API 'SI, *nx_packet_pool_create* kullanarak daha önce oluşturulmuş bir NETX ıp örneği *nx_ip_create* ve daha önce oluşturulmuş bir NETX paket havuzu gerektirir. NetX POP3 Istemcisi TCP hizmetlerini kullandığından, aynı IP örneğinde NetX POP3 Istemci hizmetlerini kullanmadan önce *nx_tcp_enable* çağrısıyla TCP 'nin etkinleştirilmesi gerekir. POP3 Istemcisi, sunucunun POP3 bağlantı noktasındaki bir POP3 sunucusuna bağlanmak için bir TCP yuvası kullanır. Bu, tipik olarak *bilinen 110 numaralı bağlantı noktasında ayarlanır, ancak HIÇBIR POP3 istemcisi veya sunucusu bu bağlantı noktasını kullanmak zorunda değildir.*

POP3 Istemcisini oluştururken kullanılan paket havuzunun boyutu, paket yükü ve kullanılabilir paket sayısı bakımından Kullanıcı tarafından yapılandırılabilir. Paket yalnızca POP3 Istemcisi oluştur hizmetinde kullanılıyorsa, paket yükünün Kullanıcı adı ve parola uzunluğuna veya APOP özetine bağlı olarak 100-120 bayttan fazla olmaması gerekir. Yerel konağın Kullanıcı adına sahip kullanıcı komutu, büyük olasılıkla POP3 Istemcisi tarafından gönderilen en büyük iletidir. IP iç işlemleri TCP denetim verileri göndermek ve almak için çok büyük bir paket yükü gerektirmediğinden, nx_ip_create (IP varsayılan paket havuzunda) aynı paket havuzunu paylaşmak mümkündür.

Ancak, ağ sürücüsünün POP3 Istemci paket havuzuyla aynı paket havuzunu kullanması avantajlı olmayabilir. Genellikle, paket havuzu yükünü al yükü, POP3 Istemci iletilerinden çok daha büyük olan ağ arabiriminin IP örneği MTU 'sunu (genellikle 1500 bayt) ayarlar. Gelen POP3 iletileri genellikle çok daha büyük veriler ve giden POP3 Istemci iletileri olur

## <a name="netx-pop3-client-creation"></a>NetX POP3 Istemcisi oluşturma

POP3 Istemcisi oluşturma hizmeti, TCP yuvasını oluşturmak *nx_pop3_client_create* ve POP3 sunucusuyla bağlantı kurmak.

POP3 sunucusu ile bağlandıktan sonra POP3 Istemci uygulaması, maildrop kutusunda oturan posta öğelerinin sayısını almak için *nx_pop3_client _mail_items_get* çağırabilir:

```c
UINT nx_pop3_client_mail_items_get(NX_POP3_CLIENT *client_ptr,
                                UINT *number_mail_items,
                                ULONG *maildrop_total_size)
```

Istemci posta kutusunda bir veya daha fazla öğe varsa, uygulama belirli bir posta öğesinin boyutunu *nx_pop3_client_get_mail_item* hizmetini kullanarak alabilir:

```c
UINT nx_pop3_client_mail_item_get(NX_POP3_CLIENT *client_ptr,
                                UINT mail_item,
                                ULONG *item_size)
```

Maildrop 'daki ilk posta öğesi Dizin 1 ' dir.

Asıl e-posta iletisini almak için, uygulama, hizmet tarafından son paketin final_packet giriş bağımsız değişkeni tarafından alındığını belirten posta iletisi paketlerini almak için *nx_pop3_client_mail_item_get_message_data* hizmetini çağırabilir:

```c
UINT nx_pop3_client_mail_item_message_get(
                        NX_POP3_CLIENT *client_ptr,
                        NX_PACKET **recv_packet_ptr,
                        ULONG *bytes_retrieved,
                        UINT *final_packet)
```

Belirli bir posta öğesini silmek için uygulama, önceki *nx_pop3_client_get_mail_item* çağrısında kullanılan aynı dizinle *nx_pop3_client_mail_item_delete* çağırır.

Istemci *nx_pop3_client_delete* hizmeti kullanılarak silinebilir. Uygulamanın, *nx_packet_pool_delete* HIZMETINI kullanarak POP3 istemci paket havuzunu silme konusunda uygulamaya yönelik olduğunu göz önünde kalmaz.

## <a name="netx-pop3-client-constraints"></a>NetX POP3 Istemci kısıtlamaları

NetX POP3 Istemcisi uygulamasında bazı kısıtlamalar vardır:

1. NetX POP3 Istemcisi, kimlik doğrulama komutunu desteklemez, ancak Istemci sunucusu kimlik doğrulaması alışverişi için DIGEST-MD5 kullanarak APOP kimlik doğrulaması uygular.

1. NetX POP3 Istemcisi tüm POP3 komutlarını uygulamaz (örn. TOP veya UıDL komutları). Aşağıda, desteklediği komutların bir listesi verilmiştir:
   - NOOP
   - RSET

## <a name="netx-pop3-client-login"></a>NetX POP3 Istemcisi oturum açma

Bir NetX POP3 Istemcisinin, bir maildrop 'a erişmek için bir POP3 sunucusunda kendi kimliğini (oturum açma) doğrulaması gerekir. Bunu, Kullanıcı/GEÇIŞ komutlarını kullanarak ve POP3 sunucusunda bilinen bir Kullanıcı adı ve parola sağlayarak ya da aşağıda açıklanan APOP komutu ve MD5 özetini kullanarak yapabilir.

Kullanıcı adı genellikle tam etki alanı adıdır (bir ' @ ' karakteriyle ayrılmış bir yerel parça ve bir etki alanı adı içerir). Kullanıcı ve PASS POP3 komutlarını kullanırken, Istemci kullanıcı adını ve parolasını Internet üzerinden şifrelenmemiş şekilde gönderiyor.

Kullanıcı adı ve parola Temizleme güvenlik riskini ortadan kaldırmak için, NetX POP3 Istemcisi *nx_pop3_client_create* hizmetindeki *APOP_authentication* parametresi ayarlanarak APOP kimlik doğrulamasını kullanacak şekilde yapılandırılabilir:

```c
UINT  nxd_pop3_client_create(NX_POP3_CLIENT *client_ptr,
                            UINT APOP_authentication,
                            NX_IP *ip_ptr,
                            NX_PACKET_POOL *packet_pool_ptr,
                            NXD_ADDRESS *server_ip_address, ULONG server_port,
                            CHAR *client_name,
                            CHAR *client_password)
```

Ya da yalnızca IPv4 uygulamaları için *nx_pop3_client_create* hizmeti:

```c
UINT  nx_pop3_client_create(NX_POP3_CLIENT *client_ptr,
                            UINT APOP_authentication,
                            NX_IP *ip_ptr,
                            NX_PACKET_POOL *packet_pool_ptr,
                            ULONG server_ip_address,
                            ULONG server_port, CHAR *client_name,
                            CHAR *client_password)
```

Istemci APOP komutunu gönderdiğinde, sunucu etki alanını, yerel saati ve sunucu selamından ayıklanan işlem KIMLIĞINI ve Istemci parolasını içeren bir MD5 özeti alır. POP3 sunucusu aynı bilgileri içeren bir MD5 özeti oluşturacak ve bunun MD5 özeti Istemcinin MD5 özeti ile eşleşiyorsa, Istemcinin kimliği doğrulanır.

APOP kimlik doğrulaması başarısız olursa, NetX POP3 Istemcisi Kullanıcı/GEÇIŞ kimlik doğrulaması gerçekleştirmeye çalışır.

## <a name="the-pop3-client-maildrop"></a>POP3 Istemcisi posta bırakma

İstemci posta, bir posta kutusundaki veya "maildrop" bir POP3 sunucusunda depolanır. POP3 sunucusundaki bir Istemci maildrop, posta öğelerinin 1 tabanlı bir listesi olarak temsil edilir. Diğer bir deyişle, her postanın, Dizin 1 ' deki (sıfır değil) ilk posta öğesiyle maildrop listesindeki diziniyle başvurulur. POP3 komutları, bu listedeki dizinlerinden belirli posta öğelerine başvurur.

## <a name="the-pop3-protocol-state-machine"></a>POP3 protokol durumu makinesi

POP3 protokolü, hem Istemci hem de sunucunun POP3 oturumunun durumunu korumasını gerektirir. İlk olarak, Istemci POP3 sunucusuna bağlanmaya çalışır. Başarılı olursa, RFC 1939 tarafından tanımlanan üç farklı durum bulunan POP3 protokolüne girer. İlk durum, kendisini sunucusuna tanıtmak zorunda olduğu yetkilendirme durumudur. Yetkilendirme durumunda, POP3 Istemcisi yalnızca Kullanıcı ve GEÇIŞ komutlarını, bu sırada veya APOP komutunu verebilir.

POP3 Istemcisinin kimliği doğrulandıktan sonra, Istemci oturumu Işlem durumunu girer. Bu durumda, Istemci posta silme işlemini indirebilir ve talep edebilir. Işlem durumunda izin verilen komutlar LIST, STAT, RETR, SIL, RSET ve QUIT. Genellikle, POP3 Istemcisi bir dizi RETR komutuyla izlenen bir STAT komutu gönderir.

Istemci, çıkış komutuna ulaştıktan sonra POP3 oturumu, sunucudan TCP bağlantısını kesmeyi başlattığı güncelleştirme durumuna girer. Postayı daha sonra indirmek için, POP3 Istemci uygulaması istediğiniz `nx_pop3_client_mail_items_get` zaman arayarak maildrop 'da yeni posta olup olmadığını denetleyebilir.

### <a name="pop3-server-reply-codes"></a>POP3 sunucusu yanıt kodları

- **+ Tamam**: sunucu, istemci komutunu kabul etmek için bu yanıtı kullanır. Sunucu, ' + Tamam ' öğesinden sonra ek bilgi içerebilir, ancak posta iletisi verilerini veya LISTE ya da SIL komutlarını karşıdan yükleme durumu dışında Istemcinin bu bilgileri işleyeceğini varsaymaz. İkinci durumda, komut sonrasında ' Argument ', Istemci maildrop içindeki posta öğesinin dizinine başvurduktan sonra.

- **-Err**: sunucu, bir istemci komutunu reddetmek için bu yanıtı kullanır. Sunucu, '-ERR ' sonrasında ek bilgi gönderebilir, ancak Istemcinin bu bilgileri işleyeceğini varsayamaz.

### <a name="sample-pop3-client---server-session"></a>Örnek POP3 Istemcisi-sunucu oturumu

**Kullanıcı/GEÇIŞ kullanan temel POP3 örneği:**

```c
S: <wait for connection on TCP port 110>
C: <open connection>
S: +OK POP3 server ready <1896.697170952@dbc.mtview.ca.us>
C: USER mrose
S: +OK mrose is valid
C: PASS mvan99
S: +OK mrose is logged in
C: STAT
S: +OK 2 320
C: RETR 1
S: +OK 120 octets
S: <the POP3 server sends message 1>
S: .
C: DELE 1
S: +OK message 1 deleted
C: RETR 2
S: +OK 200 octets
S: <the POP3 server sends message 2>
S: .
C: DELE 2
S: +OK message 2 deleted
C: QUIT
S: +OK POP3 server signing off (maildrop empty)
C: <close connection>
S: <wait for next connection>
```

**APOP (ve STAT yerine LIST) kullanan temel POP3 örneği:**

```c
S: <wait for connection on TCP port 110>
C: <open connection>
S: +OK POP3 server ready <1896.697170952@dbc.mtview.ca.us>
C: APOP mrose c4c9334bac560ecc979e58001b3e22fb
S: +OK mrose's maildrop has 2 messages (320 octets)
C: LIST
S: +OK 2 messages (320 octets)
S: 1 120
S: 2 200
S: .
C: RETR 1
S: +OK 120 octets
S: <the POP3 server sends message 1>
S: .
C: DELE 1
S: +OK message 1 deleted
C: RETR 2
S: +OK 200 octets
S: <the POP3 server sends message 2>
S: .
C: DELE 2
S: +OK message 2 deleted
C: QUIT
S: +OK dewey POP3 server signing off (maildrop empty)
C: <close connection>
S: <wait for next connection>
```

## <a name="rfcs-supported-by-netx-pop3-client"></a>NetX POP3 Istemcisi tarafından desteklenen RFC 'Ler

NetX Istemci POP3, RFC 1939 ile uyumludur.
