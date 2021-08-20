---
title: Bölüm 2 - NetX Duo MQTT Azure RTOS yükleme ve kullanma
description: Bu bölümde NetX Duo MQTT Client bileşeninin yüklenmesi, kurulumu ve kullanımıyla ilgili çeşitli sorunların açıklaması yer almaktadır.
author: philmea
ms.author: philmea
ms.date: 05/19/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 4e27a6738456a90f3d708789f51b0471868c6f9e
ms.sourcegitcommit: 4842f4cfe9e31b3ac59059f43e598eb70faebc8f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/20/2021
ms.locfileid: "122601319"
---
# <a name="chapter-2---installation-and-use-of-azure-rtos-netx-duo-mqtt-client"></a>Bölüm 2 - NetX Duo MQTT Azure RTOS yükleme ve kullanma

Bu bölümde NetX Duo MQTT istemci bileşeninin yüklenmesi, kurulumu ve kullanımıyla ilgili Azure RTOS sorunların açıklaması yer almaktadır.

## <a name="product-distribution"></a>Ürün Dağıtımı

NetX Duo için MQTT İstemcisi'ne şu bağlantıdan [https://github.com/azure-rtos/netxduo](https://github.com/azure-rtos/netxduo) bakabilirsiniz: . Paket, biri dahil olan iki kaynak dosyayı ve bu belgeyi içeren bir dosyayı içerir:

- **nxd_mqtt_client.h** NetX Duo için MQTT İstemcisi üst bilgi dosyası
- **nxd_mqtt_client.c** NetX Duo için MQTT İstemcisi için C Kaynak dosyası
- **nxd_mqtt_client.pdf** NetX Duo için MQTT İstemcisi Açıklaması
- **demo_mqtt_client.c** NetX Duo MQTT gösterimi

## <a name="mqtt-client-installation"></a>MQTT İstemcisi Yüklemesi

NetX Duo için MQTT İstemcisi'nin kullanılamı için, daha önce bahsedilen dağıtımın tamamı NetX Duo'nın yüklü olduğu dizine kopyalanır. Örneğin,*"\threadx\arm7\green"* dizinine NetX Duo yüklüyse NetX Duo MQTT Client için *nxd_mqtt_client.h* ve *nxd_mqtt_client.c* dizininin bu dizine kopyalanmış olması gerekir.

## <a name="using-mqtt-client"></a>MQTT İstemcisini Kullanma

NetX Duo için MQTT İstemcisi'nin kullanımı kolaydır. Temel olarak, ThreadX ve NetX Duo'tx_api kullanmak için uygulama kodu *tx_api.h* ve nx_api.h 'yi içeren *nxd_mqtt_client.h'yi* içermesi gerekir.  MQTT İstemcisi üst bilgi dosyaları dahil edildiktan sonra, uygulama kodu bu kılavuzun devamlarında açıklanan MQTT hizmetlerini kullanabilir. Uygulamanın derleme sürecinde *nxd_mqtt_client.c'yi* de içermesi gerekir. Bu dosyaların diğer uygulama dosyalarıyla aynı şekilde derlenmiş olması ve nesne formunun uygulamanın dosyalarıyla birlikte bağlantılı olması gerekir. NetX Duo MQTT Client'ı kullanmak için gerekenler bunlardır.

## <a name="using-mqtt-client-with-netx-secure-tls"></a>NetX Secure TLS ile MQTT İstemcisi Kullanma

MQTT istemcisini NetX Secure TLS modülüyle kullanmak için, uygulamada NetX Secure TLS modülü yüklü olmalı ve *nx_secure_tls_api.h* ile nx_crypto.h modülünü *içermesi gerekir.* MQTT kitaplığı, tanımlandığı gibi simgesiyle ***NX_SECURE_ENABLE*** gerekir.

## <a name="configuration-options"></a>Yapılandırma Seçenekleri

NetX Duo için MQTT istemcisinin birkaç yapılandırma seçeneği vardır. Aşağıda, her biri ayrıntılı olarak açıklanan tüm seçeneklerin listesi ve ardından velanmıştır. Varsayılan değerler listelenir, ancak nxd_mqtt_client.h eklenmeden *önce yeniden tanımlandır.*

- **NX_DISABLE_ERROR_CHECKING:** Tanımlandığı gibi, bu seçenek temel MQTT istemci hata denetimlerini kaldırır. Genellikle uygulama hata ayıklandıktan sonra kullanılır.
- **NX_SECURE_ENABLE:** Tanımlı, MQTT İstemcisi TLS desteğiyle yerleşiktir.
Bu simgenin tanımlanması için NetX Secure TLS modülünün yüklü olması gerekir.
*NX_SECURE_ENABLE* varsayılan olarak etkin değildir.**
- **NXD_MQTT_REQUIRE_TLS:** Tanımlı, uygulamanın MQTT aracıya bağlanmak için TLS kullanması gerekir. Bu özellik için *NX_SECURE_ENABLE* gerekir. Varsayılan olarak, bu simge tanımlanmamıştır.
- **NXD_MQTT_MAXIMUM_TRANSMIT_QUEUE_DEPTH:** Tanımlı, MQTT aktarım kuyruğu derinliği etkindir. Pozitif tamsayı olmalıdır.
- **NXD_MQTT_MAX_TOPIC_NAME_LENGTH:** Kullanım dışı.
- **NXD_MQTT_MAX_MESSAGE_LENGTH:** Kullanım dışı.
- **NXD_MQTT_KEEPALIVE_TIMER_RATE:** ThreadX zamanlayıcı tıklarında MQTT zamanlayıcı oranını tanımlar. Bu süreölçer, son MQTT denetim iletisi gönderilmeden bu yana geçen zamanı izlemek için kullanılır ve canlı tutma süresinin dolmadan önce bir MQTT PINGREQ iletisi gönderir. İstemci aracıya etkin tutma süreölçeri değer kümesiyle bağlanırsa bu zamanlayıcı etkinleştirilir. Varsayılan değer, TX_TIMER_TICKS_PER_SECOND saniyelik süreölçer olan varsayılan değerdir.
- **NXD_MQTT_PING_TIMEOUT_DELAY:** MQTT istemcisinin MQTT PINGREQ'yi gönderdikten sonra aracıdan PINGRESP için bekleyeceği zamanı tanımlar. Bu zaman aşımı gecikmesi sonrasında pingRESP alınmazsa, istemci aracıyı yanıt vermiyor olarak kabul eder ve kendisiyle aracı bağlantısını keser. Varsayılan PING zaman aşımı gecikmesi TX_TIMER_TICKS_PER_SECOND bir saniyedir.
- **NXD_MQTT_SOCKET_TIMEOUT:** Zamanlayıcı saat işaretlerindeki MQTT sunucusuyla bağlantı kesileri sırasında TCP yuvası bağlantı kesme çağrısında zaman out(zaman) tanımlar. Varsayılan değer, NX_WAIT_FOREVER.

## <a name="sample-mqtt-program"></a>Örnek MQTT programı

Aşağıdaki program basit bir MQTT uygulamasını göstermektedir. Kolaylık olması için dönüş kodlarının başarılı olduğu varsayılır, bu nedenle başka hata denetimi yapılmaz.

```c
#define LOCAL_SERVER_ADDRESS (IP_ADDRESS(192, 168, 1, 81))

/*******************************************************/
/* IOT MQTT Client Example                             */
/*******************************************************/
#define DEMO_STACK_SIZE 2048
#define CLIENT_ID_STRING "mytestclient"
#define MQTT_CLIENT_STACK_SIZE 4096
#define STRLEN(p) (sizeof(p) - 1)

/* Declare the MQTT thread stack space. */
static ULONG mqtt_client_stack[MQTT_CLIENT_STACK_SIZE / sizeof(ULONG)];

/* Declare the MQTT client control block. */
static NXD_MQTT_CLIENT mqtt_client;

/* Define the symbol for signaling a received message. */

/* Define the test threads. */

#define TOPIC_NAME "topic"

#define MESSAGE_STRING "This is a message. "

/* Define the priority of the MQTT internal thread. */
#define MQTT_THREAD_PRIORTY 2

/* Define the MQTT keep alive timer for 5 minutes */
#define MQTT_KEEP_ALIVE_TIMER 300
#define QOS0 0
#define QOS1 1

/* Declare event flag, which is used in this demo. */
TX_EVENT_FLAGS_GROUP mqtt_app_flag;
#define DEMO_MESSAGE_EVENT 1
#define DEMO_ALL_EVENTS 3

/* Declare buffers to hold message and topic. */
static UCHAR message_buffer[NXD_MQTT_MAX_MESSAGE_LENGTH];
static UCHAR topic_buffer[NXD_MQTT_MAX_TOPIC_NAME_LENGTH];

/* Declare the disconnect notify function. */
static VOID my_disconnect_func(NXD_MQTT_CLIENT *client_ptr)
{
    printf("client disconnected from server\n");
}

static VOID my_notify_func(NXD_MQTT_CLIENT* client_ptr, UINT number_of_messages)
{
    tx_event_flags_set(&mqtt_app_flag, DEMO_MESSAGE_EVENT, TX_OR);
    return;
}

static ULONG error_counter;
void demo_mqtt_client_local(NX_IP *ip_ptr, NX_PACKET_POOL *pool_ptr)
{
    UINT status;
    NXD_ADDRESS server_ip;
    ULONG events;
    UINT topic_length, message_length;

    /* Create MQTT client instance. */
    nxd_mqtt_client_create(&mqtt_client, "my_client",
        CLIENT_ID_STRING, STRLEN(CLIENT_ID_STRING), ip_ptr, pool_ptr,
        (VOID*)mqtt_client_stack, sizeof(mqtt_client_stack),
        MQTT_THREAD_PRIORTY, NX_NULL, 0);

    /* Register the disconnect notification function. */
    nxd_mqtt_client_disconnect_notify_set(&mqtt_client, my_disconnect_func);

    /* Create an event flag for this demo. */
    status = tx_event_flags_create(&mqtt_app_flag, "my app event");
    server_ip.nxd_ip_version = 4;
    server_ip.nxd_ip_address.v4 = LOCAL_SERVER_ADDRESS;

    /* Start the connection to the server. */
    nxd_mqtt_client_connect(&mqtt_client, &server_ip, NXD_MQTT_PORT, 
        MQTT_KEEP_ALIVE_TIMER, 0, NX_WAIT_FOREVER);

    /* Subscribe to the topic with QoS level 0. */
    nxd_mqtt_client_subscribe(&mqtt_client, TOPIC_NAME, STRLEN(TOPIC_NAME),
        QOS0);

    /* Set the receive notify function. */
    nxd_mqtt_client_receive_notify_set(&mqtt_client, my_notify_func);

    /* Publish a message with QoS Level 1. */
    nxd_mqtt_client_publish(&mqtt_client, TOPIC_NAME,
        STRLEN(TOPIC_NAME), (CHAR*)MESSAGE_STRING, 
        STRLEN(MESSAGE_STRING), 0, QOS1, NX_WAIT_FOREVER);

    /* Now wait for the broker to publish the message. */
    tx_event_flags_get(&mqtt_app_flag, DEMO_ALL_EVENTS,
        TX_OR_CLEAR, &events, TX_WAIT_FOREVER);

    if(events & DEMO_MESSAGE_EVENT)
    {
        nxd_mqtt_client_message_get(&mqtt_client, topic_buffer,
            sizeof(topic_buffer), &topic_length, message_buffer,
            sizeof(message_buffer), &message_length);

        topic_buffer[topic_length] = 0;

        message_buffer[message_length] = 0;

        printf("topic = %s, message = %s\n", topic_buffer, message_buffer);
    }

    /* Now unsubscribe the topic. */
    nxd_mqtt_client_unsubscribe(&mqtt_client, TOPIC_NAME,
        STRLEN(TOPIC_NAME));

    /* Disconnect from the broker. */
    nxd_mqtt_client_disconnect(&mqtt_client);

    /* Delete the client instance, release all the resources. */
    nxd_mqtt_client_delete(&mqtt_client);
    return;
}
```
