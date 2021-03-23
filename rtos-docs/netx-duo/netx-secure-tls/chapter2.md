---
title: Bölüm 2-Azure RTOS NetX güvenli yükleme ve kullanımı
description: Bu bölüm, NetX güvenli bileşeninin yüklenmesiyle, kurulumuyla ve kullanımıyla ilgili çeşitli sorunların açıklamasını içerir.
author: philmea
ms.author: philmea
ms.date: 06/04/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: b3ef82bd113518b35105fb2eefe23bd3e755ca06
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104826951"
---
# <a name="chapter-2---installation-and-use-of-azure-rtos-netx-secure"></a>Bölüm 2-Azure RTOS NetX güvenli yükleme ve kullanımı

Bu bölümde, Azure RTOS NetX güvenli bileşeninin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.

## <a name="product-version-number"></a>Ürün sürüm numarası

Kullanıcı nx_secure_tls. h ' de aşağıdaki sembolleri bularak ürün sürüm numarasını doğrulayamayabilir:

***NETX_SECURE_MAJOR_VERSION***

***NETX_SECURE_MINOR_VERSION***

Hizmet paketi sürümleri, hizmet paketi numarasını göstermek için tanımlanan aşağıdaki simgeye sahiptir:

***NETX_SECURE_SERVICE_PACK_VERSION***

## <a name="product-distribution"></a>Ürün dağıtımı

NetX güvenli, adresinde bulunabilir [https://github.com/azure-rtos/netx](https://github.com/azure-rtos/netx) . Paket, kaynak dosyaları, içerme dosyaları ve bu belgeyi içeren bir PDF dosyasını aşağıdaki gibi içerir:

- **nx_secure_tls_api. h** NetX güvenli TLS için ortak API üst bilgi dosyası
- **nx_secure_tls_user. h** Kullanıcı NetX güvenli TLS için üst bilgi dosyasını tanımlıyor
- **nx_secure_tls_port. h** NetX güvenli için platforma özgü tanımlar
- **nx_secure_tls. h** NetX güvenli TLS için üst bilgi dosyası
- **nx_secure_tls&#42;. c/h** NetX güvenli TLS için C/H kaynak dosyaları
- **nx_crypto&#42;. c/h** NetX güvenli şifrelemesi için C/H kaynak dosyaları
- **nx_secure_x509&#42;. c/h** X. 509.440 dijital sertifikaları için C/H kaynak dosyaları.
- **demo_netx_secure_tls. c** NetX güvenli TLS tanıtımı için C kaynak dosyası
- **NetX_Secure_User_Guide.pdf** NetX güvenli ürününün PDF açıklaması

> [!NOTE]
> Nx_crypto * dosyaları, NetX güvenli üst dizininin bir alt dizinindeki farklı donanım platformları için sağlanır.

## <a name="netx-secure-installation"></a>NetX güvenli yükleme

NetX güvenliğini sağlamak için, daha önce bahsedilen dağıtımın tamamı, NetX 'in yüklü olduğu aynı dizin düzeyine kopyalanmalıdır. Örneğin, "*\Threadx\arm7\netx*" dizininde NETX yüklüyse, *nx_secure * *.* dizinler "*\Threadx\arm7\netxsecure*" dizinine kopyalanmalıdır.

## <a name="using-netx-secure"></a>NetX güvenli kullanma

NetX güvenli TLS kullanımı basittir. Temel olarak uygulama kodu, ThreadX ve NetX kullanmak için *tx_api. h* ve *nx_api. h* dahil *nx_secure_tls_api. h* 'yi içermelidir. *Nx_secure_tls_api. h* dahil olduğunda, uygulama kodu daha sonra bu kılavuzda belirtilen NETX güvenli işlev çağrılarını yapabilir. Uygulamanın Ayrıca, ** * nx_secure* içeri aktarması gerekir. dosyaları NetXSecure kitaplığına ve platforma özgü *nx_crypto * *.* dosyaları Netxşifre kitaplığı içine ekleyin.

## <a name="small-example-system-tls-client"></a>Küçük örnek sistem (TLS Istemcisi)

Aşağıdaki gibi, Şekil 1,1 ' de NetX güvenli kullanılması için ne kadar kolay bir örnek açıklanmıştır. Bu, şifreleme için yazılım şifreleme modüllerini (donanıma özgü değil) kullanarak basit bir TLS Istemcisi gösterir. OpenSSL ters yankı sunucusu (OpenSSL s_server-Rev) ile çalışmak üzere tasarlanmıştır.

Bu örneği çalıştırmak için, hedef sunucunuzun sertifikasının kimliğini doğrulamak üzere bir X. 509.952 CA sertifikasına ihtiyacınız olacağını unutmayın. OpenSSL örneği için, basit bir 2 düzeyi PKI (kök CA sertifikası-> >sunucu sertifikası) yeterli olacaktır. "Trusted_ca_data" dizisini CA sertifikanızın DER kodlu ikili sürümüyle doldurmanız ve "trusted_ca_length" değişkenini sertifikanızın gerçek uzunluğunu yansıtacak şekilde güncelleştirmeniz gerekir.

Ayrıca, donanımınızın ağ sürücüsüne da ihtiyacınız vardır (nx_ip_create çağrısındaki "nx_driver_xx" parametresini değiştirin).

```C
#include "tx_api.h"
#include "nx_api.h"
#include "nx_secure_tls_api.h"
#include "nx_secure_x509.h"

/* Define the size of our application stack. */
#define     DEMO_STACK_SIZE             4096

/* Define the remote server IP address using NetX IP_ADDRESS macro. */
#define     REMOTE_SERVER_IP_ADDRESS    IP_ADDRESS(192, 168, 1, 1)

/* Define the IP address for this device. */
#define     DEVICE_IP_ADDRESS           IP_ADDRESS(192, 168, 1, 2)

/* Define the remote server port. 443 is the HTTPS default. */
#define     REMOTE_SERVER_PORT          443

/* Define the ThreadX and NetX object control blocks...  */

NX_PACKET_POOL          pool_0;
NX_IP                   ip_0;
NX_TCP_SOCKET tcp_socket;
NX_SECURE_TLS_SESSION tls_session;
NX_SECURE_X509_CERT certificate;

/* Define an HTTP request to be sent to the HTTPS web server not defined here but
  represented by the ellipsis. */
UCHAR http_request[] = { "GET /example.html HTTP/1.1"  };

/* Define the IP thread's stack area.  */
ULONG ip_thread_stack[3 * 1024 / sizeof(ULONG)];

/* Define packet pool for the demonstration.  */
#define NX_PACKET_POOL_SIZE ((1536 + sizeof(NX_PACKET)) * 32)

ULONG packet_pool_area[NX_PACKET_POOL_SIZE/sizeof(ULONG) + 64 / sizeof(ULONG)];

/* Define the ARP cache area.  */
ULONG arp_space_area[512 / sizeof(ULONG)];

/* Define the TLS Client thread.  */
ULONG             tls_client_thread_stack[6 * 1024 / sizeof(ULONG)];
TX_THREAD         tls_client_thread;
void              client_thread_entry(ULONG thread_input);

/* Define the TLS packet reassembly buffer. */
UCHAR tls_packet_buffer[18000];

/* Define the metadata area for TLS cryptography. The actual size needed can be
   Ascertained by calling nx_secure_tls_metadata_size_calculate.
*/
UCHAR tls_crypto_metadata[18000];

/* Pointer to the TLS ciphersuite table that is included in the platform-specific
   cryptography subdirectory. The table maps the cryptographic routines for the
   platform to function pointers usable by the TLS library.
*/
extern const NX_SECURE_TLS_CRYPTO nx_crypto_tls_ciphers_ecc;
extern const USHORT nx_crypto_ecc_supported_groups[];
extern const NX_CRYPTO_METHOD *nx_crypto_ecc_curves[];
extern const UINT nx_crypto_ecc_supported_groups_size;

/* Binary data for the TLS Client X.509 trusted root CA certificate, ASN.1 DER-
   encoded. A trusted certificate must be provided for TLS Client applications
   (unless X.509 authentication is disabled) or TLS will treat all certificates as
   untrusted and the handshake will fail.
*/

/* DER-encoded binary certificate, not defined here but represented by the ellipsis,
   for the sake of brevity. */
const UCHAR trusted_ca_data[] = { … };
const UINT trusted_ca_length = 0x574;

/* Define the application – initialize drivers and TCP/IP setup.
   NOTE: the variable “status” should be checked after every API call. Most error
         checking has been omitted for clarity. */
void    tx_application_define(void *first_unused_memory)
{
UINT  status;

   /* Initialize the NetX system.  */
   nx_system_initialize();

   /* Create a packet pool. Check status for errors. */
   status =  nx_packet_pool_create(&pool_0, "NetX Main Packet Pool", 1536,
                                   (ULONG*)(((int)packet_pool_area + 64) & ~63) ,
                                   NX_PACKET_POOL_SIZE);

   /* Create an IP instance for the specific target. Check status for errors. This
      call is not completely defined. Please see other demo files for proper usage
      of the nx_ip_create call. */
   status = nx_ip_create(&ip_0, "NetX IP Instance 0",
                         DEVICE_IP_ADDRESS ,
                         0xFFFFFF00UL,
                         &pool_0, nx_driver_xx,
                         (UCHAR*)ip_thread_stack,
                         sizeof(ip_thread_stack),
                         1);

   /* Enable ARP and supply ARP cache memory for IP Instance 0. Check status for
       errors. */
   status =  nx_arp_enable(&ip_0, (void *)arp_space_area, sizeof(arp_space_area));

   /* Enable TCP traffic. Check status for errors. */
   status =  nx_tcp_enable(&ip_0);

   status =  nx_ip_fragment_enable(&ip_0);

   /* Initialize the NetX Secure TLS system.  */
   nx_secure_tls_initialize();

    /* Create the TLS client thread to start handling incoming requests. */
   tx_thread_create(&tls_client_thread, "TLS Client thread", client_thread_entry, 0,
                     tls_client_thread_stack, sizeof(tls_client_thread_stack),
                     16, 16, 4, TX_AUTO_START);
   return;
}

/* Thread to handle the TLS Client instance. */
void client_thread_entry(ULONG thread_input)
{
UINT       status;
ULONG       actual_status;
NX_PACKET *send_packet;
NX_PACKET *receive_packet;
UCHAR receive_buffer[100];
ULONG bytes;
ULONG server_ipv4_address;

    /* We are not using the thread input parameter so suppress compiler warning. */
    NX_PARAMETER_NOT_USED(thread_input);

   /* Ensure the IP instance has been initialized.  */
   status =  nx_ip_status_check(&ip_0, NX_IP_INITIALIZE_DONE, &actual_status,
                                 NX_IP_PERIODIC_RATE);

   /* Create a TCP socket to use for our TLS session.  */
   status =  nx_tcp_socket_create(&ip_0, &tcp_socket, "TLS Client Socket",
                                  NX_IP_NORMAL, NX_FRAGMENT_OKAY,
                                  NX_IP_TIME_TO_LIVE, 8192, NX_NULL, NX_NULL);

   /* Create a TLS session for our socket. This sets up the TLS session object for
          later use */
   status =  nx_secure_tls_session_create(&tls_session,
                                          &nx_crypto_tls_ciphers_ecc,
                                          tls_crypto_metadata,
                                          sizeof(tls_crypto_metadata));

   /* Initialize ECC parameters for this session. */
   status = nx_secure_tls_ecc_initialize(&tls_session,
                                             nx_crypto_ecc_supported_groups,
                                             nx_crypto_ecc_supported_groups_size,
                                             nx_crypto_ecc_curves);

   /* Set the packet reassembly buffer for this TLS session. */
   status = nx_secure_tls_session_packet_buffer_set(&tls_session, tls_packet_buffer,
                                                    sizeof(tls_packet_buffer));

   /* Initialize an X.509 certificate with our CA root certificate data. */
   nx_secure_x509_certificate_initialize(&certificate, trusted_ca_data,
                                         trusted_ca_length, NX_NULL, 0, NX_NULL, 0,
                                         NX_SECURE_X509_KEY_TYPE_NONE);

   /* Add the initialized certificate as a trusted root certificate. */
   nx_secure_tls_trusted_certificate_add(&tls_session, &certificate);

   /* Setup this thread to open a connection on the TCP socket to a remote server.
      The IP address can be used directly or it can be obtained via DNS or other
      means.*/
   server_ipv4_address = REMOTE_SERVER_IP_ADDRESS;
   status = nx_tcp_client_socket_connect(&tcp_socket, server_ipv4_address,
                                         REMOTE_SERVER_PORT, NX_WAIT_FOREVER);

   /* Start the TLS Session using the connected TCP socket. This function will
      ascertain from the TCP socket state that this is a TLS Client session. */
   status = nx_secure_tls_session_start(&tls_session, &tcp_socket,
                                         NX_WAIT_FOREVER);

    /* Allocate a TLS packet to send an HTTP request over TLS (HTTPS). */
    status = nx_secure_tls_packet_allocate(&tls_session, &pool_0, &send_packet,
                                          NX_WAIT_FOREVER);

    /* Populate the packet with our HTTP request. */
    nx_packet_data_append(send_packet, http_request, sizeof(http_request), &pool_0,
                          NX_WAIT_FOREVER);


   /* Send the HTTP request over the TLS Session, turning it into HTTPS. */
   status = nx_secure_tls_session_send(&tls_session, send_packet, NX_WAIT_FOREVER);

   /* If the send fails, you must release the packet.  */
   if (status != NX_SUCCESS)
   {
         /* Release the packet since the packet was not sent.  */
         nx_packet_release(send_packet);
   }

   /* Receive the HTTP response and any data from the server. */
   status = nx_secure_tls_session_receive(&tls_session, &receive_packet,
   NX_WAIT_FOREVER);
   if (status == NX_SUCCESS)
   {
       /* Extract the data we received from the remote server. */
       status = nx_packet_data_extract_offset(receive_packet, 0, receive_buffer,
                                             100,  &bytes);
        /* Display the response data. */
       receive_buffer[bytes] = 0;
       printf("Received data: %s\n", receive_buffer);

        /* Release the packet when done with it. */
       nx_packet_release(receive_packet);
   }

   /* End the TLS session now that we have received our HTTPS/HTML response. */
   status = nx_secure_tls_session_end(&tls_session, NX_WAIT_FOREVER);

   /* Check for errors to make sure the session ended cleanly. */

   /* Disconnect the TCP socket. */
   status =  nx_tcp_socket_disconnect(&tcp_socket, NX_WAIT_FOREVER);

}
```

**Şekil 1,1 NetX ile NetX güvenli kullanımı örneği**

## <a name="small-example-system-tls-web-server"></a>Küçük örnek sistem (TLS Web sunucusu)

Aşağıda görüntülenen ve basit bir TLS Web sunucusunu (HTTPS) gösteren şekil 1,1 ' de, NetX güvenli kullanmanın ne kadar kolay olduğunu gösteren bir örnek.

Bu örneği çalıştırmak için, sunucunuzu TLS istemcilere tanıtmak üzere bir X. 509.952 sertifikasına ihtiyacınız olacağını unutmayın. Çoğu Web browiçin, kendinden imzalı basit bir sertifika yeterli olmalıdır. Tarayıcınız sunucu kimliğini doğrulayamayacak ve bazı durumlarda sunucu<sup>3</sup>' e YÖNELIK bir TLS/https bağlantısı kuramamakta olabilir. "Certificate_data" dizisini Sunucu sertifikanızın DER kodlu ikili sürümüyle doldurmanız ve "certificate_length" değişkenini sertifikanızın gerçek uzunluğunu yansıtacak şekilde güncelleştirmeniz gerekir. Ayrıca, "private_key" dizisini, RSA anahtarı için PKCS # 1 ve ECC anahtarları için RFC 5915 kullanılarak biçimlendirilen sertifikanızın özel anahtarının DER kodlu bir sürümü ile doldurmanız gerekir. "Private_key_length" değişkenini anahtar verilerinizin gerçek uzunluğuyla birlikte girin.

> [!IMPORTANT]
> Bazı tarayıcılar (özellikle Chrome tarayıcısının bazı sürümleri) otomatik olarak imzalanan sertifikaları reddedebilirler. Bu durumda, sunucu sertifikanızı imzalamak için kullanılan bir kök CA sertifikası ile 2 düzeyli bir PKI oluşturabilirsiniz. Bu durumda, kök CA sertifikası tarayıcınıza güvenilen bir kök sertifika olarak yüklenir. !!! ÖNEMLI: işiniz bittiğinde ve üretim uygulamaları için kullanmadan kök CA sertifikanızı tarayıcınızdan kaldırın!!!

Ayrıca, donanımınızın ağ sürücüsüne da ihtiyacınız vardır (nx_ip_create çağrısındaki "nx_driver_xx" parametresini değiştirin).

```C
#include "tx_api.h"
#include "nx_api.h"
#include "nx_secure_tls_api.h"
#include "nx_secure_x509.h"

#define     DEMO_STACK_SIZE         4096

/* Define the IP address for this device. */
#define     DEVICE_IP_ADDRESS             IP_ADDRESS(192, 168, 1, 2)

/* Define the ThreadX and NetX object control blocks...  */

NX_PACKET_POOL          pool_0;
NX_IP                   ip_0;
NX_TCP_SOCKET tcp_socket;
NX_SECURE_TLS_SESSION tls_session;
NX_SECURE_X509_CERT certificate;

/* Define the IP thread's stack area.  */
ULONG ip_thread_stack[3 * 1024 / sizeof(ULONG)];

/* Define packet pool for the demonstration.  */
#define NX_PACKET_POOL_SIZE ((1536 + sizeof(NX_PACKET)) * 32)

ULONG packet_pool_area[NX_PACKET_POOL_SIZE/sizeof(ULONG) + 64 / sizeof(ULONG)];

/* Define the ARP cache area.  */
ULONG arp_space_area[512 / sizeof(ULONG)];


/* Define the TLS Server thread.  */
ULONG             tls_server_thread_stack[6 * 1024 / sizeof(ULONG)];
TX_THREAD         tls_server_thread;
void              server_thread_entry(ULONG thread_input);

/* Define the TLS packet reassembly buffer. */
UCHAR tls_packet_buffer[18000];

/* Define the metadata area for TLS cryptography. The actual size needed can be
   Ascertained by calling nx_secure_tls_metadata_size_calculate.
*/
UCHAR tls_crypto_metadata[18000];

/* Pointer to the TLS ciphersuite table that is included in the platform-specific
   cryptography subdirectory. The table maps the cryptographic routines for the
   platform to function pointers usable by the TLS library.
*/
extern const NX_SECURE_TLS_CRYPTO nx_crypto_tls_ciphers_ecc;
extern const USHORT nx_crypto_ecc_supported_groups[];
extern const NX_CRYPTO_METHOD *nx_crypto_ecc_curves[];
extern const UINT nx_crypto_ecc_supported_groups_size;

/* Binary data for the TLS Server X.509 certificate, ASN.1 DER-encoded. Note that the
   certificate data and private key data is represented by an ellipsis for the sake
   of brevity.
*/
const UCHAR certificate_data[] = { … }; /* DER-encoded binary certificate. */
const UINT certificate_length = 0x574;

/* Binary data for the TLS Server Private Key, from private key
   file generated at the time of the X.509 certificate creation. ASN.1 DER-encoded. */
const UCHAR private_key[] = { … }; /* DER-encoded private key file (PKCS#1 RSA or ECC) */
const UINT private_key_length = 0x40;

/* Define some HTML data (web page) with an HTTPS header to serve to connecting
   clients. */
UCHAR html_data[] = { "HTTP/1.1 200 OK\r\n" \
        "Date: Tue, 19 May 2020 23:59:59 GMT\r\n" \
        "Content-Type: text/html\r\n" \
        "Content-Length: 200\r\n\r\n" \
        "<html>\r\n"\
        "<body>\r\n"\
        "<b>Hello NetX Secure User!</b>\r\n"\
        "This is a simple webpage\r\n"\
        "served up using NetX Secure!\r\n"\
        "</body>\r\n"\
        "</html>\r\n" };

/* Define the application – initialize drivers and TCP/IP setup.  */
void    tx_application_define(void *first_unused_memory)
{
UINT  status;


    /* Initialize the NetX system.  */
    nx_system_initialize();

    /* Create a packet pool. Check status for errors. */
    status =  nx_packet_pool_create(&pool_0, "NetX Main Packet Pool", 1536,
                                    (ULONG*)(((int)packet_pool_area + 64) & ~63) ,
                                    NX_PACKET_POOL_SIZE);

    /* Create an IP instance for the specific target. Check status for errors. */
    status = nx_ip_create(&ip_0, "NetX IP Instance 0",
                          DEVICE_IP_ADDRESS,
                          0xFFFFFF00UL,
                          &pool_0, nx_driver_xx,
                          (UCHAR*)ip_thread_stack,
                          sizeof(ip_thread_stack),
                          1);

    /* Enable ARP and supply ARP cache memory for IP Instance 0. Check status for
         errors. */
    status =  nx_arp_enable(&ip_0, (void *)arp_space_area, sizeof(arp_space_area));

    /* Enable TCP traffic. Check status for errors. */
    status =  nx_tcp_enable(&ip_0);

    status =  nx_ip_fragment_enable(&ip_0);

    /* Initialize the NetX Secure TLS system.  */
    nx_secure_tls_initialize();

    /* Create the TLS server thread to start handling incoming requests. */
    tx_thread_create(&tls_server_thread, "TLS Server thread", server_thread_entry, 0,
                   tls_server_thread_stack, sizeof(tls_server_thread_stack),
                   16, 16, 4, TX_AUTO_START);
    return;
}

/* Thread to handle the TLS Server instance. */
void server_thread_entry(ULONG thread_input)
{
UINT       status;
ULONG      actual_status;
NX_PACKET *send_packet;
NX_PACKET *receive_packet;
UCHAR receive_buffer[100];
ULONG bytes;

    NX_PARAMETER_NOT_USED(thread_input);

    /* Ensure the IP instance has been initialized.  */
    status =  nx_ip_status_check(&ip_0, NX_IP_INITIALIZE_DONE, &actual_status,
                                 NX_IP_PERIODIC_RATE);

    /* Create a TCP socket to use for our TLS session.  */
    status =  nx_tcp_socket_create(&ip_0, &tcp_socket, "TLS Server Socket",
                                   NX_IP_NORMAL, NX_FRAGMENT_OKAY,
                                   NX_IP_TIME_TO_LIVE, 8192, NX_NULL, NX_NULL);

    /* Create a TLS session for our socket.  */
    status =  nx_secure_tls_session_create(&tls_session,
                                        &nx_crypto_tls_ciphers_ecc,
                                        tls_crypto_metadata,
                                        sizeof(tls_crypto_metadata));

    status = nx_secure_tls_ecc_initialize(&tls_session,
                                          nx_crypto_ecc_supported_groups,
                                          nx_crypto_ecc_supported_groups_size,
                                          nx_crypto_ecc_curves);

     /* Set the packet reassembly buffer for this TLS session. */
     status = nx_secure_tls_session_packet_buffer_set(&tls_session, tls_packet_buffer,
                                                      sizeof(tls_packet_buffer));

    /* Initialize an X.509 certificate and private ECC key for our TLS Session. */
    nx_secure_x509_certificate_initialize(&certificate, certificate_data, NX_NULL, 0,
                                          certificate_length, private_key,
                                          private_key_length,
                                          NX_SECURE_X509_KEY_TYPE_EC_DER);

    /* Add the initialized certificate as a local identity certificate. */
    nx_secure_tls_local_certificate_add(&tls_session, &certificate);


    /* Setup this thread to listen on the TCP socket.
       Port 443 is standard for HTTPS. */
    status =  nx_tcp_server_socket_listen(&ip_0, 443, &tcp_socket, 5, NX_NULL);

    while(1)
     {
         /* Accept a client TCP socket connection.  */
         status =  nx_tcp_server_socket_accept(&tcp_socket, NX_WAIT_FOREVER);

         /* Start the TLS Session using the connected TCP socket. */
         status = nx_secure_tls_session_start(&tls_session, &tcp_socket,
                                              NX_WAIT_FOREVER);

         /* Receive the HTTPS request. */
         status = nx_secure_tls_session_receive(&tls_session, &receive_packet,
                                                NX_WAIT_FOREVER);

if (status == NX_SUCCESS)
      {
         /* Extract the HTTP request information from the HTTPS request. */
            status = nx_packet_data_extract_offset(receive_packet, 0, receive_buffer,
                                                  100, &bytes);
         /* Display the HTTP request data. */
            receive_buffer[bytes] = 0;
            printf("Received data: %s\n", receive_buffer);

         /* Release the packet when done with it */
            nx_packet_release(receive_packet);
      }

         /* Allocate a TLS packet to send HTML data back to client. */
         status = nx_secure_tls_packet_allocate(&tls_session, &pool_0, &send_packet,
                                                NX_WAIT_FOREVER);

         /* Populate the packet with our HTTP response and HTML web page data. */
         nx_packet_data_append(send_packet, html_data, sizeof(html_data), &pool_0,
                               NX_WAIT_FOREVER);

         /* Send the HTTP response over the TLS Session, turning it into HTTPS. */
         status = nx_secure_tls_session_send(&tls_session, send_packet,
                                                 NX_WAIT_FOREVER);

         /* If the send fails, you must release the packet.  */
         if (status != NX_SUCCESS)
         {
              /* Release the packet since it was not sent.  */
              nx_packet_release(send_packet);
         }

         /* End the TLS session now that we have sent our HTTPS/HTML response. */
         status = nx_secure_tls_session_end(&tls_session, NX_WAIT_FOREVER);

         /* Check for errors to make sure the session ended cleanly! */

         /* Disconnect the TCP socket so we can be ready for the next request. */
         status =  nx_tcp_socket_disconnect(&tcp_socket, NX_WAIT_FOREVER);

         /* Unaccept the server socket.  */
         status =  nx_tcp_server_socket_unaccept(&tcp_socket);

         /* Setup server socket for listening again.  */
         status =  nx_tcp_server_socket_relisten(&ip_0, 443, &tcp_socket);
     }
}
```

**Şekil 1,2 NetX ile NetX güvenli kullanımı örneği**

## <a name="a-note-on-tls-session-error-recovery"></a>TLS oturum hatası kurtarmasıyla ilgili bir notta

Yukarıda açıklanan örnek sistemler, sırasıyla bir TLS Istemcisi ve sunucusu için temel anahatları göstermektedir, ancak hata işlemenin açıklık yok edilir. Ancak, güvenlik TLS 'nin bir parçası, hata koşullarının doğru işlenmesine bağımlıdır. Genellikle, en önemli olası sorunlar TLS yığınının kendisi içinde işlenir, ancak TLS uygulamasının TLS uygulamasında işlenmemiş olan TLS hatalarını doğru şekilde yanıtlaması ve kurtarmaması önemlidir.

Doğru hata işleme için gerekli mantığı göstermek üzere aşağıdaki işlev, TLS hatalarını doğru bir şekilde işlemek için kullanılabilecek tipik bir API hizmetleri koleksiyonunu gösterir ve bir hata durumuyla karşılaşıldığında TLS durumunu sorunsuz bir şekilde sıfırlayabilir. Belirtilen bölümden farklı olarak, mantık hem TLS Istemcisi hem de TLS sunucu örnekleri için geçerlidir.

İşlevindeki en önemli API çağrılarının, TLS oturumunu veya el sıkışmasını düzgün bir şekilde kapatan *nx_secure_tls_session_reset* ve TLS oturum durumunu temizleyen ve bu da tls_session denetim yapısı örneğinin yenı bir TLS oturumu için yeniden kullanılabilmesi için *nx_secure_tls_session_end* hizmetlere olduğunu unutmayın. *Nx_secure_tls_session_reset* , sertifikalar veya atanan arabellekler gibi kullanıcı tarafından yapılandırılan durumu temizlemez, bu da oturumun *nx_secure_tls_session_create* çağrılmadan yeniden kullanılmasına izin verir. Tüm TLS oturum durumunu tamamen temizlemek için, bunun yerine hizmet *nx_secure_tls_session_delete* kullanılabilir.

```C
/* Define a helper function to clean up a broken TLS session (to be called on any
   error from nx_secure_tls_session_start onwards). Note that the variables
   tls_session, tcp_socket, and ip_0 are global in the above examples. */
VOID tls_session_error_cleanup(VOID)
{
UINT status;
UINT alert_level, alert_value;

      /* If we got an error back from a TLS API call, there may be an alert from the
         remote host. Extract the alert level and value to print out. Note that the TLS
         API will return NX_SECURE_TLS_ALERT_RECEIVED (0x114) if an alert was received.
         For other error codes the alert value and level are not valid. */
      status = nx_secure_tls_session_alert_value_get(&tls_session, &alert_level,
                                                     &alert_value);
      if(status)
      {
         printf("Pointer error in getting alert value.\n");
      }
      else
      {
         printf("Alert recieved. Value: %d, Level: %d\n", alert_value, alert_level);
      }

      /* End the TLS session. This is required to properly shut down the TLS
         connection. */
      status = nx_secure_tls_session_end(&tls_session, NX_WAIT_FOREVER);

      /* If the session did not shut down cleanly, this is a possible security issue. */
      if (status)
      {
         printf("Error in TLS session end: %x\n", status);
      }

      /* Reset the TLS session to re-use the control structure for the next connection.
         This API service resets the TLS session state but does not remove user-
         configured options such as certificates, PSKs, buffers, and cipher routines. */
      nx_secure_tls_session_reset(&tls_session);

      /* Disconnect the TCP socket, closing the connection. */
      status =  nx_tcp_socket_disconnect(&tcp_socket, NX_WAIT_FOREVER);

      /* Check for error.  */
      if (status)
      {
           printf("Error in TCP socket close: %x\n", status);
      }

   /* The following code applies only to a TLS server instance. */
   #if NX_SECURE_TLS_SERVER
      /* Unaccept the server socket.  */
      status =  nx_tcp_server_socket_unaccept(&tcp_socket);

      /* Check for error.  */
      if (status)
      {
           printf("Error in TCP socket unaccept: %x\n", status);
      }

      /* Setup server socket for listening again.  */
      status =  nx_tcp_server_socket_relisten(&ip_0, DEVICE_SERVER_PORT, &tcp_socket);

      /* Check for error.  */
      if (status)
      {
           printf("Error in TCP socket relisten: %x\n", status);
      }
#endif
} /* End function. */
```

## <a name="configuration-options"></a>Yapılandırma seçenekleri

NetX güvenli oluşturmak için birkaç yapılandırma seçeneği vardır. Aşağıda, her birinin ayrıntılı olarak açıklandığı tüm seçeneklerin bir listesi verilmiştir:

| Tanımlayın | Anlamı |
|----------------------|------------------------------------------------|
| **NX_SECURE_DISABLE_ERROR_CHECKING**                | Tanımlı, bu seçenek temel NetX güvenli hata denetimini kaldırır. Genellikle uygulamanın hata ayıklaması yapıldıktan sonra kullanılır. |
| **NX_CRYPTO_MAX_RSA_MODULUS_SIZE**                  | Tanımlı, bu seçenek bit cinsinden beklenen maksimum RSA mod sayısını verir. 4096 bit mod için varsayılan değer 4096 ' dir. Diğer değerler 3072, 2048 veya 1024 (önerilmez) olabilir. |
| **NX_SECURE_ALLOW_SELF_SIGNED_CERTIFICATES**        | Bu seçenek, TLS 'nin otomatik olarak imzalanan sertifikaları uzak bir konaktan kabul etmesine izin verir. Varsayılan olarak, TLS otomatik olarak imzalanan sunucu sertifikalarını güvenlik önlemi olarak reddeder. Bu makro tanımlanmışsa, otomatik olarak imzalanan sertifikaların kabul edilmesi için güvenilen depoya hala eklenmesi gerekir. |
| **NX_SECURE_ENABLE_CLIENT_CERTIFICATE_VERIFY**      | Tanımlı, bu seçenek<sup>TLS sunucuları için</sup>Isteğe bağlı X. 509.440 Istemci sertifikası doğrulamasını mümkün bir şekilde sunar.  |
| **NX_SECURE_ENABLE_PSK_CIPHERSUITES**               | Tanımlı, bu seçenek önceden paylaşılan anahtar (PSK) işlevselliği sunar. Dijital sertifikaları devre dışı bırakır. |
| **NX_SECURE_TLS_CLIENT_DISABLED**                   | Tanımlı, bu seçenek TLS Istemci moduyla ilgili tüm TLS yığın kodunu kaldırır, kod ve veri kullanımını azaltır. |
| **NX_SECURE_TLS_SERVER_DISABLED**                   | Tanımlı, bu seçenek, TLS sunucu moduyla ilgili tüm TLS yığın kodunu kaldırır, kod ve veri kullanımını azaltır.  |
| **NX_SECURE_DISABLE_ECC_CIPHERSUITE**               | Tanımlı, bu seçenek Eliptik Eğri Şifreleme (ECC) cipherpaketlerine yönelik tüm TLS mantığını kaldırır. Bu ciphersuites, TLS 1,2 ve önceki sürümlerde isteğe bağlıdır ve bunların devre dışı bırakılması, önemli kod ve veri boyutu azalmasına neden olabilir.|
| **NX_SECURE_TLS_ENABLE_TLS_1_3**                    | Tanımlı, bu seçenek TLSv 1.3 modunu etkinleştirmesine izin vermez. TLS 1,3, en yeni TLS sürümüdür ve varsayılan olarak devre dışıdır. |
| **NX_SECURE_TLS_ENABLE_TLS_1_0**                    | Tanımlı, bu seçenek eski TLSv 1.0 modunu sunar. TLSv 1.0 kullanımdan kalktı, bu nedenle yalnızca eski uygulamalarla geriye dönük uyumluluk için etkinleştirilmelidir. |
| **NX_SECURE_TLS_ENABLE_TLS_1_1**                    | Tanımlı, bu seçenek eski TLSv 1.1 modunu sunar. TLSv 1.1 kullanımdan kalkmıştır, bu nedenle yalnızca eski uygulamalarla geriye dönük uyumluluk için etkinleştirilmelidir. |
| **NX_SECURE_TLS_DISABLE_TLS_1_1**                   | Tanımlı, bu seçenek TLSv 1.1 modunu devre dışı bırakır. Varsayılan olarak tanımlanmıştır. TLSv 1.1 yalnızca daha güvenli TLSv 1.2<sup>5</sup>kullanımı için devre dışı bırakılmıştır.  |
| **NX_SECURE_X509_STRICT_NAME_COMPARE**              | Bu seçenek, sertifika arama ve doğrulama için X. 509.440 sertifikaları için katı ayırt edici ad karşılaştırmayı mümkün bir şekilde sunar. Varsayılan değer yalnızca ayırt edici adların ortak ad alanlarını karşılaştıramaktır.|
| **NX_SECURE_X509_USE_EXTENDED_DISTINGUISHED_NAMES** | Bu seçenek, X. 509.440 sertifikaları için ek bellek kullanımı masrafındaki isteğe bağlı X. 509.952 ayırt edici ad alanlarını mümkün bir şekilde sunar. |

4. Bu seçeneğin yalnızca kodun uygulamayla bağlantılandırılmasına izin olduğunu unutmayın. Özelliğin, Istemci sertifikası doğrulamasını kullanmak için nx_secure_tls_session_client_verify_enable API hizmeti ile etkinleştirilmesi veya nx_secure_tls_session_x509_client_verify_configure kullanılarak yapılandırılması gerekir.

5. Yalnızca TLS 1,0 veya TLS 1,1 kullanılıyorsa TLSv 1.2 'yi devre dışı bırakmak de mümkün olduğunu unutmayın. Ancak, bu önerilmez ve doğrudan desteklenmez.
