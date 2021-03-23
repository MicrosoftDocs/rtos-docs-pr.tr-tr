---
title: Bölüm 2-Azure RTOS NetX PPPoE Istemcisini yükleme ve kullanma
description: Bu bölümde, Azure RTOS NetX PPPoE Istemci bileşeninin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.
author: philmea
ms.author: philmea
ms.date: 07/13/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 17d910647db7b207280b3fbd9e90c468293a8e67
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104826638"
---
# <a name="chapter-2---installation-and-use-of-azure-rtos-netx-pppoe-client"></a>Bölüm 2-Azure RTOS NetX PPPoE Istemcisini yükleme ve kullanma

Bu bölümde, Azure RTOS NetX PPPoE Istemci bileşeninin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.

## <a name="product-distribution"></a>Ürün dağıtımı

NetX için PPPoE Istemcisi, adresinde bulunabilir [https://github.com/azure-rtos/netx](https://github.com/azure-rtos/netx) . Paket aşağıdaki dosyaları içerir:

 - **nx_pppoe_client. h** NetX için PPPoE Istemcisi üst bilgi dosyası
 - **nx_pppoe_client. c** NetX için PPPoE Istemcisi için C kaynak dosyası
 - **nx_pppoe_client.pdf** NetX için PPPoE Istemcisinin PDF açıklaması
 - **demo_netx_pppoe_client. c** NetX PPPoE Istemci tanıtımı

## <a name="pppoe-client-installation"></a>PPPoE Istemci yüklemesi

NetX için PPPoE Istemcisini kullanabilmeniz için, daha önce bahsedilen dağıtımın tamamı, NetX 'in yüklü olduğu dizine kopyalanmalıdır. Örneğin, *"\threadx\arm7\green"* dizininde NETX yüklüyse, *nx_pppoe_client. h* ve *nx_pppoe_client. c* dosyaları bu dizine kopyalanmalıdır.

## <a name="using-pppoe-client"></a>PPPoE Istemcisini kullanma

NetX için PPPoE Istemcisini kullanmak kolaydır. Temel olarak, uygulama kodu sırasıyla ThreadX ve NetX kullanmak için *tx_api. h* ve *nx_api. h* dahil *nx_pppoe_client.* h içermelidir. *Nx_pppoe_client. h* dahil olduğunda, uygulama kodu daha sonra bu kılavuzda belirtilen PPPoE istemci işlev çağrılarını yapabilir. Uygulama, yapı işlemine *nx_pppoe_client. c* de içermelidir. Bu dosya, diğer uygulama dosyalarıyla aynı şekilde derlenmelidir ve nesne formu, uygulamanın dosyalarıyla birlikte bağlanmalıdır. Bu, NetX PPPoE Istemcisini kullanmak için gereklidir.

## <a name="small-example-system"></a>Küçük örnek sistem

Aşağıda, The NetX PPPoE Istemcisinin nasıl kullanıldığını gösteren bir örnek verilmiştir. Şekil 1,1. Bu örnekte, *nx_pppoe_client. h* olan PPPoE istemci içerme dosyası 50. satırda getirilir. Ardından, PPPoE Istemcisi, 238 satırındaki *"thread_0_entry"* içinde oluşturulur. IP örneği oluşturulduktan sonra PPPoE Istemcisinin oluşturulması gerektiğini unutmayın. IP örneği ve PPP örneği oluşturulur ve line142-220 başlatılır. *"Pppoe_client"* PPPoE istemci denetim bloğu, daha önce satır 75 ' de genel bir değişken olarak tanımlandı. Gönderme ve alma işlevleri satır 238 ' de ayarlanır.

Genel olarak, PPPoE modülünün PPP modülüyle birlikte kullanılması gerekir. Bu örnekte, PPP Istemcisi içerme dosyası *nx_ppp. h* , 49. satırda getirilir. Ardından, 164. satırda PPP Istemcisi oluşturulur. Satır 172 PPP paketini göndermek için işlevi ayarlayın. Satır 179-190 IP adreslerini ayarlayın ve PAP protokolünü tanımlayın. Satır 104-129 PAP protokolü için Kullanıcı adı ve parola ayarlayın.

PPPoE oturumu kurulduktan sonra. Uygulama, 264 satırındaki oturum bilgilerini (sunucu MAC adresi ve oturum kimliği) almak için *nx_pppoe_client_session_get* çağırabilir. PPP veya uygulama, 283 satırındaki PPPoE paketini göndermek için *nx_pppoe_client_session_packet_send* çağırabilir.

Uygulama artık PPP trafiğini işlemesiz, uygulama PPPoE oturumunu sonlandırmak için *nx_pppoe_client_session_terminate* çağırabilir.

Bu örnekte, PPPoE Istemcisi normal IP Stack ile aynı anda çalışır ve bir Ethernet sürücüsünü paylaşır. 155. satırdaki normal IP örneği için aynı Ethernet sürücüsünü ve @. satırdaki PPPoE Istemci 298 örneğini geçirin.

> [!NOTE]
> Fiziksel üstbilgiyi doldurmak için yeterli alan sağlamak üzere **NX_PHYSICAL_HEADER** 24 ' e yeniden tanımlayın. Fiziksel üst bilgi: 14 (Ethernet üstbilgisi) + 6 (PPPoE üstbilgisi) + 2 (PPP üstbilgisi) + 2 (dört baytlık hizalama).

```c
  1 /**************************************************************************/
  2 /**************************************************************************/
  3 /**                                                                       */
  4 /** NetX PPPoE Client stack Component                                     */
  5 /**                                                                       */
  6 /**   This is a small demo of the high-performance NetX PPPoE Client      */
  7 /**   stack. This demo includes IP instance, PPPoE Client and PPP Client  */
  8 /**   stack. Create one IP instance includes two interfaces to support    */
  9 /**   for normal IP stack and PPPoE Client, PPPoE Client can use the      */
 10 /**   mutex of IP instance to send PPPoE message when share one Ethernet  */
 11 /**   driver. PPPoE Client work with normal IP instance at the same time. */
 12 /**                                                                       */
 13 /**   Note1: Substitute your Ethernet driver instead of                   */
 14 /**   _nx_ram_network_driver before run this demo                         */
 15 /**                                                                       */
 16 /**   Note2: Prerequisite for using PPPoE.                                */
 17 /**   Redefine NX_PHYSICAL_HEADER to 24 to ensure enough space for filling*/
 18 /**   in physical header. Physical header:14(Ethernet header)             */
 19 /**    + 6(PPPoE header) + 2(PPP header) + 2(four-byte aligment)          */
 20 /**                                                                       */
 21 /**************************************************************************/
 22 /**************************************************************************/
 23
 24
 25       /*****************************************************************/
 26       /*                          NetX Stack                           */
 27       /*****************************************************************/
 28
 29                                             /***************************/
 30                                             /*        PPP Client       */
 31                                             /***************************/
 32
 33                                             /***************************/
 34                                             /*       PPPoE Client      */
 35                                             /***************************/
 36       /***************************/         /***************************/
 37       /*    Normal Ethernet Type */         /*    PPPoE Ethernet Type  */
 38       /***************************/         /***************************/
 39       /***************************/         /***************************/
 40       /*       Interface 0       */         /*       Interface 1       */
 41       /***************************/         /***************************/
 42
 43       /*****************************************************************/
 44       /*                       Ethernet Dirver                         */
 45       /*****************************************************************/
 46
 47 #include   "tx_api.h"
 48 #include   "nx_api.h"
 49 #include   "nx_ppp.h"
 50 #include   "nx_pppoe_client.h"
 51
 52 /* Defined NX_PPP_PPPOE_ENABLE if use Express Logic's PPP, since PPP module has been modified
       to match PPPoE moduler under this definition.  */
 53 #ifdef NX_PPP_PPPOE_ENABLE
 54
 55 /* If the driver is not initialized in other module, define NX_PPPOE_CLIENT_INITIALIZE_DRIVER_ENABLE
       to initialize the driver in PPPoE module .
 56    In this demo, the driver has been initialized in IP module.  */
 57 #ifndef NX_PPPOE_CLIENT_INITIALIZE_DRIVER_ENABLE
 58
 59 /* Define the block size.  */
 60 #define     NX_PACKET_POOL_SIZE     ((1536 + sizeof(NX_PACKET)) * 30)
 61 #define     DEMO_STACK_SIZE         2048
 62 #define     PPPOE_THREAD_SIZE       2048
 63
 64 /* Define the ThreadX and NetX object control blocks...  */
 65 TX_THREAD               thread_0;
 66
 67 /* Define the packet pool and IP instance for normal IP instnace.  */
 68 NX_PACKET_POOL          pool_0;
 69 NX_IP                   ip_0;
 70
71 /* Define the PPP Client instance.  */
 72 NX_PPP                  ppp_client;
 73
 74 /* Define the PPPoE Client instance.  */
 75 NX_PPPOE_CLIENT         pppoe_client;
 76
 77 /* Define the counters.  */
 78 CHAR                    *pointer;
 79 ULONG                   error_counter;
 80
 81 /* Define thread prototypes.  */
 82 void    thread_0_entry(ULONG thread_input);
 83
 84 /***** Substitute your PPP driver entry function here *********/
 85 extern void    _nx_ppp_driver(NX_IP_DRIVER *driver_req_ptr);
 86
 87 /***** Substitute your Ethernet driver entry function here *********/
 88 extern void    _nx_ram_network_driver(NX_IP_DRIVER *driver_req_ptr);
 89
 90 /* Define the porting layer function for Express Logic's PPP to simulate TTP's PPP.
 91    Functions to be provided by PPP for calling by the PPPoE Stack.  */
 92 void    ppp_client_packet_send(NX_PACKET *packet_ptr);
 93 void    pppoe_client_packet_receive(NX_PACKET *packet_ptr);
 94
 95 /* Define main entry point.  */
 96
 97 int main()
 98 {
 99
100     /* Enter the ThreadX kernel.  */
101     tx_kernel_enter();
102 }
103
104 UINT generate_login(CHAR *name, CHAR *password)
105 {
106
107     /* Make a name and password, called "myname" and "mypassword".  */
108     name[0] = 'm';
109     name[1] = 'y';
110     name[2] = 'n';
111     name[3] = 'a';
112     name[4] = 'm';
113     name[5] = 'e';
114     name[6] = (CHAR) 0;
115
116     password[0] = 'm';
117     password[1] = 'y';
118     password[2] = 'p';
119     password[3] = 'a';
120     password[4] = 's';
121     password[5] = 's';
122     password[6] = 'w';
123     password[7] = 'o';
124     password[8] = 'r';
125     password[9] = 'd';
126     password[10] = (CHAR) 0;
127
128     return(NX_SUCCESS);
129 }
130
131 /* Define what the initial system looks like.  */
132
133 void    tx_application_define(void *first_unused_memory)
134 {
135
136 UINT    status;
137
138     /* Setup the working pointer.  */
139     pointer =  (CHAR *) first_unused_memory;
140
141     /* Initialize the NetX system.  */
142     nx_system_initialize();
143
144     /* Create a packet pool for normal IP instance.  */
145     status = nx_packet_pool_create(&pool_0, "NetX Main Packet Pool",
146                                    (1536 + sizeof(NX_PACKET)),
147                                    pointer, NX_PACKET_POOL_SIZE);
148     pointer = pointer + NX_PACKET_POOL_SIZE;
149
150     /* Check for error.  */
151     if (status)
152         error_counter++;
153
154     /* Create an normal IP instance.  */
155     status = nx_ip_create(&ip_0, "NetX IP Instance", IP_ADDRESS(192, 168, 100, 44), 0xFFFFFF00UL,
156                           &pool_0, _nx_ram_network_driver, pointer, 2048, 1);
157     pointer = pointer + 2048;
158
159     /* Check for error.  */
160     if (status)
161         error_counter++;
162
163     /* Create the PPP instance.  */
164     status = nx_ppp_create(&ppp_client, "PPP Instance", &ip_0, pointer, 2048, 1,
165                            &pool_0, NX_NULL, NX_NULL); pointer = pointer + 2048;
166
167     /* Check for PPP create error.   */
168     if (status)
169         error_counter++;
170
171     /* Set the PPP packet send function.  */
172     status = nx_ppp_packet_send_set(&ppp_client, ppp_client_packet_send);
173
174     /* Check for PPP packet send function set error.   */
175     if (status)
176         error_counter++;
177
178     /* Define IP address. This PPP instance is effectively the client since it doesn't have
           any IP addresses. */
179     status = nx_ppp_ip_address_assign(&ppp_client, IP_ADDRESS(0, 0, 0, 0), IP_ADDRESS(0, 0, 0, 0));
180
181     /* Check for PPP IP address assign error.   */
182     if (status)
183         error_counter++;
184
185     /* Setup PAP, this PPP instance is effectively the since it generates the name and password
           for the peer..  */
186     status = nx_ppp_pap_enable(&ppp_client, generate_login, NX_NULL);
187
188     /* Check for PPP PAP enable error.  */
189     if (status)
190         error_counter++;
191
192     /* Attach an interface for PPP.  */
193     status = nx_ip_interface_attach(&ip_0, "Second Interface For PPP", IP_ADDRESS(0, 0, 0, 0), 0,
                                        nx_ppp_driver);
194
195     /* Check for error.  */
196     if (status)
197         error_counter++;
198
199     /* Enable ARP and supply ARP cache memory for Normal IP Instance.  */
200     status = nx_arp_enable(&ip_0, (void *) pointer, 1024);
201     pointer = pointer + 1024;
202
203     /* Check for ARP enable errors.  */
204     if (status)
205         error_counter++;
206
207     /* Enable ICMP */
208     status = nx_icmp_enable(&ip_0);
209     if(status)
210         error_counter++;
211
212     /* Enable UDP traffic.  */
213     status =  nx_udp_enable(&ip_0);
214     if (status)
215         error_counter++;
216
217     /* Enable TCP traffic.  */
218     status =  nx_tcp_enable(&ip_0);
219     if (status)
220         error_counter++;
221
222     /* Create the main thread.  */
223     tx_thread_create(&thread_0, "thread 0", thread_0_entry, 0,
224                      pointer, DEMO_STACK_SIZE,
225                      4, 4, TX_NO_TIME_SLICE, TX_AUTO_START);
226     pointer =  pointer + DEMO_STACK_SIZE;
227
228 }
229
230 /* Define the test threads.  */
231
232 void    thread_0_entry(ULONG thread_input)
233 {
234 UINT    status;
235 ULONG   ip_status;
236
237     /* Create the PPPoE instance.  */
238     status =  nx_pppoe_client_create(&pppoe_client, (UCHAR *)"PPPoE Client",  &ip_0,  0,
        &pool_0, pointer, PPPOE_THREAD_SIZE, 4, _nx_ram_network_driver, pppoe_client_packet_receive);
239     pointer = pointer + PPPOE_THREAD_SIZE;
240     if (status)
241     {
242         error_counter++;
243         return;
244     }
245
246     /* Establish PPPoE Client sessione.  */
247     status = nx_pppoe_client_session_connect(&pppoe_client, NX_WAIT_FOREVER);
248     if (status)
249     {
250         error_counter++;
251         return;
252     }
253
254     /* Wait for the link to come up.  */
255     status = nx_ip_interface_status_check(&ip_0, 1, NX_IP_ADDRESS_RESOLVED,
                                              &ip_status, NX_WAIT_FOREVER);
256     if (status)
257     {
258         error_counter++;
259         return;
260     }
261
262     /* Get the PPPoE Server physical address and Session ID after establish PPPoE Session.  */
263     /*
264     status = nx_pppoe_client_session_get(&pppoe_client, &server_mac_msw,
                                             &server_mac_lsw, &session_id);
265     if (status)
266         error_counter++;
267     */
268 }
269
270 /* PPPoE Client receive function.  */
271 void    pppoe_client_packet_receive(NX_PACKET *packet_ptr)
272 {
273
274     /* Call PPP Client to receive the PPP data fame.  */
275     nx_ppp_packet_receive(&ppp_client, packet_ptr);
276 }
277
278 /* PPP Client send function.  */
279 void    ppp_client_packet_send(NX_PACKET *packet_ptr)
280 {
281
282     /* Directly Call PPPoE send function to send out the data through PPPoE module.  */
283     nx_pppoe_client_session_packet_send(&pppoe_client, packet_ptr);
284 }
285 #endif /* NX_PPPOE_CLIENT_INITIALIZE_DRIVER_ENABLE  */
286
287 #endif /* NX_PPP_PPPOE_ENABLE  */
```

**Şekil 1,1 NetX ile PPPoE Istemci kullanımı örneği**

## <a name="configuration-options"></a>Yapılandırma seçenekleri

NetX için PPPoE Istemcisi oluşturmaya yönelik birkaç yapılandırma seçeneği vardır. Aşağıdaki listede her biri ayrıntılı açıklanmıştır:

- **NX_DISABLE_ERROR_CHECKING** Tanımlı, bu seçenek temel PPPoE Istemci hata denetimini kaldırır. Genellikle uygulamanın hata ayıklaması yapıldıktan sonra kullanılır.
- **NX_PPPOE_CLIENT_INITIALIZE_DRIVER_ENABLE** Tanımlanmışsa, özelliğin PPPoE modülünde Ethernet sürücüsünü başlatmasını sağlar. Varsayılan olarak devre dışı bırakılır.
- **NX_PPPOE_CLIENT_THREAD_TIME_SLICE** PPPoE Istemci iş parçacığı için zaman dilimi seçeneği. Varsayılan olarak, bu değer TX_NO_TIME_SLICE.
- **NX_PPPOE_CLIENT_PADI_INIT_TIMEOUT** Bu, ilk yeniden iletme PADI paketlerine yönelik beklemeyi tanımlar. Varsayılan olarak, bu değer 1 saniyedir.
- **NX_PPPOE_CLIENT_PADI_COUNT** Bu, bağlantının bozuk olduğu kabul etmeden önce kaç PADI iletme deposunun izin verileceğini tanımlar. Varsayılan olarak, bu değer 4 ' dir.
- **NX_PPPOE_CLIENT_PADR_INIT_TIMEOUT** Bu, PADR paketlerinin ilk yeniden iletilmesi için beklemeyi tanımlar. Varsayılan olarak, bu değer 1 saniyedir.
- **NX_PPPOE_CLIENT_PADR_COUNT** Bu, bağlantı bozuk kabul etmeden önce kaç PADR iletim deposunun izin verileceğini tanımlar. Varsayılan olarak, bu değer 4 ' dir.
- **NX_PPPOE_CLIENT_MAX_AC_NAME_SIZE** Bu, AC adının maksimum boyutunu tanımlar. Varsayılan olarak, bu değer 32 ' dir.
- **NX_PPPOE_CLIENT_MAX_AC_COOKIE_SIZE** Bu, AC tanımlama bilgisinin en büyük boyutunu tanımlar. Varsayılan olarak, bu değer 32 ' dir.
- **NX_PPPOE_CLIENT_MAX_RELAY_SESSION_ID_SIZE** Bu, maksimum geçiş-oturum kimliği boyutunu tanımlar. Varsayılan olarak, bu değer 12 ' dir.
- **NX_PPPOE_CLIENT_MIN_PACKET_PAYLOAD_SIZE** PPPoE Istemcisi için en düşük paket yükü boyutunu belirtir. Paket yükü boyutu bu değerden büyükse, paket zincirinden kaçınabilirsiniz. Varsayılan olarak, bu değer 1520 (en fazla Ethernet 1500, Ethernet üstbilgisi 14, CRC 2 ve dört baytlık hizalama 4).
