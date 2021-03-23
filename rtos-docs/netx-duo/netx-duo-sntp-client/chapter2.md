---
title: Bölüm 2-Azure RTOS NetX Duo SNTP Istemcisini yükleme ve kullanma
description: Bu bölüm, NetX Duo SNTP Istemcisinin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların açıklamasını içerir.
author: philmea
ms.author: philmea
ms.date: 06/04/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: cd917e7e70ce21dbff6c8081c2ff115c0acad8a8
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104825750"
---
# <a name="chapter-2---installation-and-use-of-azure-rtos-netx-duo-sntp-client"></a>Bölüm 2-Azure RTOS NetX Duo SNTP Istemcisini yükleme ve kullanma

Bu bölümde, Azure RTOS NetX Duo SNTP Istemcisinin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.

## <a name="product-distribution"></a>Ürün dağıtımı

NetX Duo için SNTP, adresinde bulunabilir [https://github.com/azure-rtos/netxduo](https://github.com/azure-rtos/netxduo) . Paket, aşağıdaki gibi, bu belgeyi içeren iki kaynak dosya ve bir PDF dosyası içerir:

- **nxd_sntp_client. c** SNTP Istemci C kaynak dosyası  
- **nxd_sntp_client. h** SNTP Istemci üst bilgi dosyası  
- **demo_netxduo_sntp_client. c** Demo SNTP Istemci uygulaması  
- **nxd_sntp_client.pdf** NetX Duo SNTP Istemci Kullanıcı Kılavuzu  

## <a name="netx-duo-sntp-client-installation"></a>NetX Duo SNTP Istemci yüklemesi

NetX Duo için SNTP kullanmak istiyorsanız, daha önce bahsedilen dağıtımın tamamı NetX Duo 'un yüklü olduğu dizine kopyalanmalıdır. Örneğin, "*\threadx\arm7\green*" dizininde NETX Duo yüklüyse, NETX Duo SNTP istemci dosyaları *nxd_sntp_client. c* ve *nxd_sntp_client. h* (*nx_sntp_client. c* ve *nx_sntp_client. h* ) bu dizine kopyalanmalıdır.

## <a name="using-netx-duo-sntp-client"></a>NetX Duo SNTP Istemcisini kullanma

NetX Duo SNTP Istemcisini kullanmak kolaydır. Temel olarak, uygulama kodu, sırasıyla ThreadX ve NetX Duo kullanmak için *tx_api. h, fx_api. h* ve *nx_api. h* dahil *nxd_sntp_client.* h içermelidir. *Nxd_sntp_client. h* dahil olduğunda, uygulama kodu daha sonra bu KıLAVUZDA belirtilen SNTP işlev çağrılarını yapabilir. Uygulama, yapı işlemine *nxd_sntp_client. c* de içermelidir. Bu dosyalar, diğer uygulama dosyalarıyla aynı şekilde derlenmesi gerekir ve nesne formu, uygulamanın dosyalarıyla birlikte bağlanmalıdır. Bu, NetX Duo SNTP Istemcisini kullanmak için gereklidir.

> [!NOTE]
> NetX Duo SNTP Istemcisi NetX Duo UDP hizmetlerini kullandığından, SNTP hizmetlerini kullanmadan önce *nx_udp_enable* çağrısıyla UDP 'nin etkinleştirilmesi gerekir.

## <a name="small-example-system"></a>Küçük örnek sistem

NetX Duo SNTP kullanmanın bir örneği aşağıda gösterilmiştir. Bu **Örneğin, sisteminizde** olduğu gibi çalıştığını unutmayın. Belirli sistem ve donanımınız için ayarlamalar yapmanız gerekebilir. Örneğin, NetX RAM sürücüsünü gerçek sürücü işleviniz ile değiştirmeniz gerekir. Bu örnek, tam olarak tanıtım amaçlı amaçlıdır.

Bu örnekte, SNTP üstbilgi dosyası *nxd_sntp_client. h* dahil edilmiştir. SNTP Istemcisi "*tx_application_define*" içinde oluşturulur. SNTP Istemcisini oluştururken, ölüm ve artık ikinci işleyici işlevlerinin KISS 'nin isteğe bağlı olduğunu unutmayın.

Bu tanıtım, IPv6 veya IPv4 ile kullanılabilir. SNTP Istemcisini IPv6 üzerinden çalıştırmak için USE_IPV6 tanımlayın. IPv6 'nın NetX Duo içinde de etkinleştirilmesi gerekir. SNTP Istemci Konağı, NetX Duo 'da IPv6 adres doğrulaması ve ICMPv6 ve IPv6 Hizmetleri için ayarlanır. NetX Duo 'daki IPv6 desteği hakkında daha ayrıntılı bilgi için bkz. NetX Duo Kullanıcı Kılavuzu.

Ardından, tek noktaya yayın veya yayın modu için SNTP Istemcisinin başlatılmış olması gerekir.

SNTP Istemcisi başlangıçta sunucu saati güncelleştirmelerini kendi iç veri yapısına yazar. Bu, cihaz yerel saati ile aynı değildir. Cihaz yerel saati, SNTP Istemci iş parçacığını başlatmadan önce SNTP Istemcisinde temel bir zaman olarak ayarlanabilir. Bu, SNTP Istemcisi yapılandırılmışsa (NX_SNTP_CLIENT_IGNORE_MAX_ADJUST_STARTUP NX_FALSE), ilk sunucu güncelleştirmesini NX_SNTP_CLIENT_MAX_ADJUSTMENT karşılaştırmak için (varsayılan değer 180 milisaniye) yararlıdır. Aksi takdirde, SNTP Istemcisi ilk yerel saati sunucudan ilk güncelleştirmeyi aldığında doğrudan ayarlar.

Temel bir süre, *nx_sntp_client_set_local_time* HIZMETI kullanılarak SNTP istemcisine uygulanır.

SNTP Istemcisi, sırasıyla tek noktaya yayın ve yayın modu için başlatılır. Belirli bir Aralık (tek noktaya yayın yoklama aralığından biraz daha az) için uygulama, geçerli saatin saniye ve milisaniyesini artırdığımız "gerçek zaman saatinin" *nx_sntp_client_set_local_time* kullanarak SNTP istemci yerel saatini güncelleştirir. Her aralıktan sonra uygulama, SNTP sunucusundan güncelleştirmeleri düzenli olarak denetler. *Nx_sntp_client_receiving _updates* HIZMETI, SNTP istemcisinin Şu anda geçerli güncelleştirmeleri aldığını doğrular. Bu durumda, *nx_sntp_client_get_local_time_extended* hizmetini kullanarak en son güncelleştirme zamanı alınır.

SNTP istemcisi, *nx_sntp_client_stop* hizmeti kullanılarak herhangi bir zamanda durdurulabilir ve bu örnek, SNTP istemcisinin artık geçerli güncelleştirmeleri almadığını algılar. Istemciyi yeniden başlatmak için uygulama, tek noktaya yayın veya yayın başlatma hizmetini çağırmalıdır ve sonra tek noktaya yayın veya yayın çalıştırma Hizmetleri 'ni çağırmalıdır. SNTP Istemci iş parçacığı görevi durdurulduğunda, SNTP Istemcisi gerekirse SNTP sunucularını ve modlarını (tek noktaya yayın veya yayın) değiştirebilir, örneğin önceki SNTP sunucusu çalışmıyor gibi görünür.

```c
/* 
   This is a small demo of the NetX SNTP Client on the high-performance NetX
   TCP/IP stack. This demo relies on Thread, NetX and NetX SNTP Client API to
   execute the Simple Network Time Protocol in unicast and broadcast modes.  
 */

#include <stdio.h>
#include "nx_api.h"
#include "nx_ip.h"
#include "nxd_sntp_client.h"
                
/* Define SNTP packet size. */
#define NX_SNTP_CLIENT_PACKET_SIZE      (NX_UDP_PACKET + 100)

/* Define SNTP packet pool size. */
#define NX_SNTP_CLIENT_PACKET_POOL_SIZE      (4 * (NX_SNTP_CLIENT_PACKET_SIZE + 
                                                            sizeof(NX_PACKET)))

/* Define how often the demo checks for SNTP updates. */
#define DEMO_PERIODIC_CHECK_INTERVAL      (1 * NX_IP_PERIODIC_RATE) 

/* Define how often we check on SNTP server status. 
   We expect updates from the SNTP server about every hour using 
   the SNTP Client defaults. For testing
   make this (much) shorter. */
#define CHECK_SNTP_UPDATES_TIMEOUT       (180 * NX_IP_PERIODIC_RATE) 

/* Set up generic network driver for demo program. */
void    _nx_ram_network_driver(struct NX_IP_DRIVER_STRUCT *driver_req);

/* Application defined services of the NetX SNTP Client. */

UINT leap_second_handler(NX_SNTP_CLIENT *client_ptr, 
                                UINT leap_indicator);
UINT kiss_of_death_handler(NX_SNTP_CLIENT *client_ptr, 
                                        UINT KOD_code);
VOID time_update_callback(NX_SNTP_TIME_MESSAGE *time_update_ptr, 
                                       NX_SNTP_TIME *local_time);


/* Set up client thread and network resources. */

NX_PACKET_POOL      client_packet_pool;
NX_IP               client_ip;
TX_THREAD           demo_client_thread;
NX_SNTP_CLIENT      demo_sntp_client;
TX_EVENT_FLAGS_GROUP sntp_flags;

#define DEMO_SNTP_UPDATE_EVENT  1

/* Configure the SNTP Client to use IPv6. If not enabled, the 
   Client will use IPv4.  Note: IPv6 must be enabled in NetX Duo
   for the Client to communicate over IPv6.    */
#ifdef FEATURE_NX_IPV6
/* #define USE_IPV6 */
#endif /* FEATURE_NX_IPV6 */


/* Configure the SNTP Client to use unicast SNTP. */
#define USE_UNICAST


#define CLIENT_IP_ADDRESS       IP_ADDRESS(192,2,2,66)
#define SERVER_IP_ADDRESS       IP_ADDRESS(192,2,2,92)
#define SERVER_IP_ADDRESS_2     SERVER_IP_ADDRESS

/* Set up the SNTP network and address index; */
UINT     iface_index =0;
UINT     prefix = 64;   
UINT     address_index;

/* Set up client thread entry point. */
void    demo_client_thread_entry(ULONG info);

/* Define main entry point.  */
int main()
{
    /* Enter the ThreadX kernel.  */
    tx_kernel_enter();
    return 0;
}

/* Define what the initial system looks like.  */
void    tx_application_define(void *first_unused_memory)
{

UINT     status;
UCHAR    *free_memory_pointer;


    free_memory_pointer = (UCHAR *)first_unused_memory;

    /* Create client packet pool. */
    status =  nx_packet_pool_create(&client_packet_pool, 
                                "SNTP Client Packet Pool",
                                NX_SNTP_CLIENT_PACKET_SIZE, 
                                free_memory_pointer, 
                                NX_SNTP_CLIENT_PACKET_POOL_SIZE);

    /* Check for errors. */
    if (status != NX_SUCCESS)
    {

        return;
    }

    /* Initialize the NetX system. */
    nx_system_initialize();

    /* Update pointer to unallocated (free) memory. */
    free_memory_pointer =  free_memory_pointer + NX_SNTP_CLIENT_PACKET_POOL_SIZE;

    /* Create Client IP instances */
    status = nx_ip_create(&client_ip, "SNTP IP Instance", 
                                        CLIENT_IP_ADDRESS, 
                                        0xFFFFFF00UL, 
                                        &client_packet_pool, 
                                       _nx_ram_network_driver, 
                                       free_memory_pointer, 2048, 1);
    
    /* Check for error. */
    if (status != NX_SUCCESS)
    {

        return;
    }

    free_memory_pointer =  free_memory_pointer + 2048;

#ifndef NX_DISABLE_IPV4
    /* Enable ARP and supply ARP cache memory. */
    status =  nx_arp_enable(&client_ip, (void **) free_memory_pointer, 2048);

    /* Check for error. */
    if (status != NX_SUCCESS)
    {

        return;
    }
#endif /* NX_DISABLE_IPV4  */

    /* Update pointer to unallocated (free) memory. */
    free_memory_pointer = free_memory_pointer + 2048;
    
    /* Enable UDP for client. */
    status =  nx_udp_enable(&client_ip);
    
    /* Check for error. */
    if (status != NX_SUCCESS)
    {

        return;
    }

#ifndef NX_DISABLE_IPV4
    status = nx_icmp_enable(&client_ip);

    /* Check for error. */
    if (status != NX_SUCCESS)
    {

        return;
    }
#endif /* NX_DISABLE_IPV4  */

    /* Create the client thread */
    status = tx_thread_create(&demo_client_thread, "SNTP Client Thread", 
                                                demo_client_thread_entry, 
                                              (ULONG)(&demo_sntp_client), 
                                                free_memory_pointer, 2048, 
                                                  4, 4, TX_NO_TIME_SLICE, 
                                                        TX_DONT_START);

    /* Check for errors */
    if (status != TX_SUCCESS)
    {

        return;
    }

    /* Create the event flags. */
    status = tx_event_flags_create(&sntp_flags, "SNTP event flags");

    /* Check for errors */
    if (status != TX_SUCCESS)
    {

        return;
    }

    /* Update pointer to unallocated (free) memory. */
    free_memory_pointer = free_memory_pointer + 2048;

    /* set the SNTP network interface to the primary interface. */
    iface_index = 0;

    /* Create the SNTP Client to run in broadcast mode.. */
status =  nx_sntp_client_create(&demo_sntp_client, &client_ip,
                           iface_index, &client_packet_pool,  
                               leap_second_handler, 
                               kiss_of_death_handler, 
                               NULL /* no random_number_generator callback */);

    /* Check for error. */
    if (status != NX_SUCCESS)
    {

        /* Bail out!*/
        return;
    }

    tx_thread_resume(&demo_client_thread);

    return;
}

/* Define size of buffer to display client's local time. */
#define BUFSIZE 50

/* Define the client thread.  */
void    demo_client_thread_entry(ULONG info)
{

UINT   status;
UINT   spin;
UINT   server_status;
ULONG  base_seconds;
ULONG  base_fraction;
ULONG  seconds, milliseconds, microseconds, fraction;
UINT   wait = 0;
UINT   error_counter = 0;
ULONG  events = 0;
#ifdef USE_IPV6
NXD_ADDRESS sntp_server_address;
NXD_ADDRESS client_ip_address;
#endif

    NX_PARAMETER_NOT_USED(info);

    /* Give other threads (IP instance) initialize first. */
    tx_thread_sleep(NX_IP_PERIODIC_RATE); 

#ifdef USE_IPV6
    /* Set up IPv6 services. */
    status = nxd_ipv6_enable(&client_ip);

    status += nxd_icmp_enable(&client_ip);

    if (status  != NX_SUCCESS)
        return;

    client_ip_address.nxd_ip_address.v6[0] = 0x20010db8;
    client_ip_address.nxd_ip_address.v6[1] = 0x0000f101;
    client_ip_address.nxd_ip_address.v6[2] = 0x0;
    client_ip_address.nxd_ip_address.v6[3] = 0x101;
    client_ip_address.nxd_ip_version = NX_IP_VERSION_V6;

    /* Set the IPv6 server address. */
    sntp_server_address.nxd_ip_address.v6[0] = 0x20010db8;  
    sntp_server_address.nxd_ip_address.v6[1] = 0x0000f101;
    sntp_server_address.nxd_ip_address.v6[2] = 0x0;
    sntp_server_address.nxd_ip_address.v6[3] = 0x00000106;
    sntp_server_address.nxd_ip_version = NX_IP_VERSION_V6;

    /* Establish the link local address for the host. The RAM driver creates
       a virtual MAC address. */
    status = nxd_ipv6_address_set(&client_ip, iface_index, NX_NULL, 10, NULL);

    /* Check for link local address set error.  */
    if (status != NX_SUCCESS) 
    {
        return;
    }

     /* Set the host global IP address. We are assuming a 64 
       bit prefix here but this can be any value (< 128). */
    status = nxd_ipv6_address_set(&client_ip, iface_index, 
                                        &client_ip_address, 
                                    prefix, &address_index);

    /* Check for global address set error.  */
    if (status != NX_SUCCESS) 
    {
        return;
    }

    /* Wait while NetX Duo validates the global and link local addresses. */
    tx_thread_sleep(5 * NX_IP_PERIODIC_RATE);

#endif

    /* Setup time update callback function. */
    nx_sntp_client_set_time_update_notify(&demo_sntp_client, 
                                        time_update_callback);

    /* Set up client time updates depending on mode. */
#ifdef USE_UNICAST

    /* Initialize the Client for unicast mode to 
       poll the SNTP server once an hour. */
#ifdef USE_IPV6
/* Use the duo service to set up the Client and set the IPv6 SNTP server.
   Note: this can take either an IPv4 or IPv6 address. */
    status = nxd_sntp_client_initialize_unicast(&demo_sntp_client, 
                                            &sntp_server_address);
#else
    /* Use the IPv4 service to set up the Client and set the IPv4 SNTP server. */
    status = nx_sntp_client_initialize_unicast(&demo_sntp_client, 
                                                SERVER_IP_ADDRESS);
#endif  /* USE_IPV6 */


#else   /* Broadcast mode */

/* Initialize the Client for broadcast mode, no roundtrip calculation
   required and a broadcast SNTP service. */
#ifdef USE_IPV6
    /* Use the duo service to initialize the Client 
       and set IPv6 SNTP all hosts multicast address. 
       (Note: This can take either an IPv4 or IPv6 address.)*/
    status = nxd_sntp_client_initialize_broadcast(&demo_sntp_client, 
                                                &sntp_server_address, 
                                                            NX_NULL);
#else

    /* Use the IPv4 service to initialize the Client and set 
       IPv4 SNTP broadcast address. */
    status = nx_sntp_client_initialize_broadcast(&demo_sntp_client,  
                                                NX_NULL, 
                                                SERVER_IP_ADDRESS);
#endif  /* USE_IPV6 */
#endif  /* USE_UNICAST */

    /* Check for error. */
    if (status != NX_SUCCESS)
    {
        return;
    }

    /* Set the base time which is approximately the number of seconds since
       the turn of the last century. If this is not available in SNTP format,
       the nx_sntp_client_utility_add_msecs_to_ntp_time service can convert
       milliseconds to fraction.  For how to compute NTP seconds from real
   time, read the NetX SNTP User Guide. Otherwise set the base time to 
   zero and set NX_SNTP_CLIENT_IGNORE_MAX_ADJUST_STARTUP to NX_TRUE for
       the SNTP CLient to accept the first time update without applying a
       minimum or maximum adjustment parameters
      (NX_SNTP_CLIENT_MIN_TIME_ADJUSTMENT and
       NX_SNTP_CLIENT_MAX_TIME_ADJUSTMENT). */

    base_seconds =  0xd2c96b90;  /* Jan 24, 2012 UTC */
    base_fraction = 0xa132db1e;

    /* Apply to the SNTP Client local time.  */
status = nx_sntp_client_set_local_time(&demo_sntp_client, base_seconds,
                                base_fraction);

    /* Check for error. */
    if (status != NX_SUCCESS)
    {
        return;
    }

    /* Run whichever service the client is configured for. */
#ifdef USE_UNICAST
    status = nx_sntp_client_run_unicast(&demo_sntp_client);
#else
    status = nx_sntp_client_run_broadcast(&demo_sntp_client);
#endif  /* USE_UNICAST */

    if (status != NX_SUCCESS)
    {
        return;
    }

    spin = NX_TRUE;

    /* Now check periodically for time changes. */
    while(spin)
    {
        /* Wait for a server update event. */
        tx_event_flags_get(&sntp_flags, DEMO_SNTP_UPDATE_EVENT, 
                                          TX_OR_CLEAR, &events, 
                                 DEMO_PERIODIC_CHECK_INTERVAL);

        if (events == DEMO_SNTP_UPDATE_EVENT)
        {

            /* Check for valid SNTP server status. */
            status = nx_sntp_client_receiving_updates(&demo_sntp_client,
                                               &server_status);

            if ((status != NX_SUCCESS) || (server_status == NX_FALSE))
            {

                /* We do not have a valid update. Skip processing any time
                   data. If this happens repeatedly, consider stopping the
                   SNTP Client thread, picking another SNTP server and
                   resuming the SNTP Client thread task (more details about
                   that in the comments at the end of this function).
                 
                   If SNTP Client configurable parameters are too restrictive,
                   such as Max Adjustment, that may also cause valid server
                   updates to be rejected. Configurable parameters, however,
                   cannot be changed at run time.
                 */
                 
                continue;
            }

            /* We have a valid update.  Get the SNTP Client time.  */
            status = nx_sntp_client_get_local_time_extended(&demo_sntp_client, 
                                                    &seconds, &fraction,  
                                                    NX_NULL, 0); 

            /* Convert fraction to microseconds. */
            nx_sntp_client_utility_fraction_to_usecs(fraction, &microseconds);

            milliseconds = ((microseconds + 500) / 1000);

            if (status != NX_SUCCESS)
            {
                printf("Internal error with getting local time 0x%x\n", 
                       status);
                error_counter++;
            }
            else
            {
                printf("\nSNTP updated\n");
                printf("Time: %lu.%03lu sec.\r\n", seconds, milliseconds);
            }

            /* Clear all events in our event flag. */
            events = 0;
        }
        else
        {

            /* No SNTP update event.             
               In the meantime, if we have an RTC we might want to check
               its notion of time. In this demo, we simulate the passage of 
               time on our 'RTC' really just the CPU counter, assuming that 
               seconds and milliseconds have previously been set to a base 
              (starting) time (as was the SNTP Client before running it) 
             */

            seconds += 1;
            milliseconds += 1;

            /* Update our timer. */
            wait += DEMO_PERIODIC_CHECK_INTERVAL;

            /* Check if it is time to display the local 'RTC' time. */
            if (wait >= CHECK_SNTP_UPDATES_TIMEOUT)
            {
                /* It is. Reset the timeout and print local time. */
                wait = 0;

                printf("Time: %lu.%03lu sec.\r\n", seconds, milliseconds);
            }           
        }
    }

/* We can stop the SNTP service if for example we think the SNTP server 
   has stopped sending updates.
     
       To restart the SNTP Client, simply call the
       nx_sntp_client_initialize_unicast or
       nx_sntp_client_initialize_broadcast using another SNTP server IP
       address as input, and resume the SNTP Client by calling
       nx_sntp_client_run_unicast or
       nx_sntp_client_run_braodcast. */
    status = nx_sntp_client_stop(&demo_sntp_client);

    if (status != NX_SUCCESS)
    {
        error_counter++;
    }

    /* When done with the SNTP Client, we delete it */
    status = nx_sntp_client_delete(&demo_sntp_client);

    return;
}


/* This application defined handler for handling an 
   impending leap second is not required by 
   the SNTP Client. The default handler below only logs the
   event for every time stamp received with the 
   leap indicator set.  */

UINT leap_second_handler(NX_SNTP_CLIENT *client_ptr, 
                                UINT leap_indicator)
{
    NX_PARAMETER_NOT_USED(client_ptr);
    NX_PARAMETER_NOT_USED(leap_indicator);

    /* Handle the leap second handler... */

    return NX_SUCCESS;
}

/* This application defined handler for handling 
   a Kiss of Death packet is not required by the SNTP Client. 
   A KOD handler should determine if the Client task should continue vs. 
   abort sending/receiving time data from its current time server, 
   and if aborting if it should remove
   the server from its active server list. 

   Note that the KOD list of codes is subject to change. The list
   below is current at the time of this software release. */

UINT kiss_of_death_handler(NX_SNTP_CLIENT *client_ptr, UINT KOD_code)
{

UINT    remove_server_from_list = NX_FALSE;
UINT    status = NX_SUCCESS;

    NX_PARAMETER_NOT_USED(client_ptr);

    /* Handle kiss of death by code group. */
    switch (KOD_code)
    {

        case NX_SNTP_KOD_RATE:
        case NX_SNTP_KOD_NOT_INIT:
        case NX_SNTP_KOD_STEP:

            /* Find another server while this one 
               is temporarily out of service.  */
            status =  NX_SNTP_KOD_SERVER_NOT_AVAILABLE;

        break;

        case NX_SNTP_KOD_AUTH_FAIL:
        case NX_SNTP_KOD_NO_KEY:
        case NX_SNTP_KOD_CRYP_FAIL:

            /* These indicate the server will not 
               service client with time updates
               without successful authentication. */


            remove_server_from_list =  NX_TRUE;

        break;


        default:

            /* All other codes. Remove server 
               before resuming time updates. */

            remove_server_from_list =  NX_TRUE;
        break;
    }

    /* Removing the server from the active server list? */
    if (remove_server_from_list)
    {

        /* Let the caller know it has to bail on 
           this server before resuming service. */
        status = NX_SNTP_KOD_REMOVE_SERVER;
    }

    return status;
}


/* This application defined handler for notifying SNTP time update event.  */

VOID time_update_callback(NX_SNTP_TIME_MESSAGE *time_update_ptr, 
                                       NX_SNTP_TIME *local_time)
{
    tx_event_flags_set(&sntp_flags, DEMO_SNTP_UPDATE_EVENT, TX_OR);
}

```

Şekil 1 NetX Duo ile SNTP Istemcisini kullanma örneği

## <a name="configuration-options"></a>Yapılandırma seçenekleri

NetX Duo SNTP Istemcisini tanımlamaya yönelik birkaç yapılandırma seçeneği vardır. Aşağıdaki listede her biri ayrıntılı açıklanmıştır:  
  

**NX_SNTP_CLIENT_THREAD_STACK_SIZE**  
Bu seçenek, Istemci iş parçacığı yığınının boyutunu ayarlar. Varsayılan NetX Duo SNTP Istemci boyutu 2048 ' dir.

**NX_SNTP_CLIENT_THREAD_TIME_SLICE**  
Bu seçenek, Scheduler 'ın Istemci iş parçacığı yürütmeye izin verdiği zaman dilimini ayarlar. Varsayılan NetX Duo SNTP Istemci boyutu TX_NO_TIME_SLICE.

**NX_SNTP_CLIENT_ THREAD_PRIORITY**  
Bu seçenek Istemci iş parçacığı önceliğini ayarlar. NetX Duo SNTP Istemci varsayılan değeri 2 ' dir.

**NX_SNTP_CLIENT_PREEMPTION_THRESHOLD**  
Bu seçenek, Istemci iş parçacığının önalım izin verdiği öncelik düzeyini ayarlar. Varsayılan NetX Duo SNTP Istemci değeri olarak ayarlanır `NX_SNTP_CLIENT_ THREAD_PRIORITY` .

**NX_SNTP_CLIENT_UDP_SOCKET_NAME**  
Bu seçenek, UDP yuva adını ayarlar. NetX Duo SNTP Istemci UDP yuva adı varsayılan değer "SNTP Istemci soketi" dir.

**NX_SNTP_CLIENT_UDP_PORT**  
Bu, Istemci yuvasının bağlandığı bağlantı noktasını ayarlar. Varsayılan NetX Duo SNTP Istemci bağlantı noktası 123 ' dir.

**NX_SNTP_SERVER_UDP_PORT**  
Bu bağlantı noktası, Istemcinin SNTP sunucusuna SNTP iletileri gönderdiği bağlantı noktasıdır. Varsayılan NetX SNTP sunucu bağlantı noktası 123 ' dir.

**NX_SNTP_CLIENT_TIME_TO_LIVE**  
Bir Istemci paketinin, atılmadan önce geçebilmesi gereken yönlendirici sayısını belirtir. Varsayılan NetX Duo SNTP Istemcisi, 0x80 olarak ayarlanır *.*

**NX_SNTP_CLIENT_MAX_QUEUE_DEPTH**  
NetX Duo SNTP Istemci yuvasında sıraya alınabilen en fazla UDP paketi sayısı (veri birimi). Alınan ek paketler, en eski paketlerin yayımlandığı anlamına gelir. Varsayılan NetX Duo SNTP Istemcisi 5 olarak ayarlanmıştır.

**NX_SNTP_CLIENT_PACKET_TIMEOUT**  
NetX Duo paket ayırması için zaman aşımı. Varsayılan NetX Duo SNTP Istemci paketi zaman aşımı değeri 1 saniyedir.

**NX_SNTP_CLIENT_NTP_VERSION**  
Istemci tarafından kullanılan SNTP sürümü NetX Duo SNTP Istemci API 'SI sürüm 4 ' ü temel alır. Varsayılan değer 3 ' dir.

**NX_SNTP_CLIENT_MIN_NTP_VERSION**  
En eski SNTP sürümü Istemci ile çalışabilir. NetX Duo SNTP Istemcisi varsayılan sürüm 3 ' dir.

**NX_SNTP_CLIENT_MIN_SERVER_STRATUM**  
İstemcinin kabul edeceği en düşük düzey (en yüksek sayısal katman düzeyi) SNTP sunucu katman. NetX Duo SNTP Istemci varsayılanı 2 ' dir.

**NX_SNTP_CLIENT_MIN_TIME_ADJUSTMENT**  
Istemcinin yerel saat saatinde yapması için milisaniye olarak en kısa süre ayarlaması. Bu, aşağıdaki zaman ayarlamaları yok sayılır. NetX Duo SNTP Istemci varsayılanı 10 ' dur.

**NX_SNTP_CLIENT_MAX_TIME_ADJUSTMENT**  
Istemcinin yerel saat saatinde yapması için milisaniye olarak en uzun süre ayarlaması. Bu tutarın üzerindeki zaman ayarlamaları için, yerel saat ayarlaması en uzun süre ayarlamasıyla sınırlıdır. NetX Duo SNTP Istemci varsayılanı 180000 (3 dakika).

**NX_SNTP_CLIENT_IGNORE_MAX_ADJUST_STARTUP**  
Bu, Istemci zaman sunucusundan ilk güncelleştirmeyi aldığında en uzun süre ayarlamasının alınmaz olmasını sağlar. Bundan sonra, en uzun süre ayarlaması zorlanır. Amaç, Istemciyi sunucu saatiyle en kısa sürede eşitlenmiş duruma getirmek için kullanılır. NetX Duo SNTP Istemci varsayılanı NX_TRUE.

**NX_SNTP_CLIENT_MAX_TIME_LAPSE**  
SNTP Istemcisi tarafından alınan geçerli bir zaman güncelleştirmesi olmadan en fazla izin verilen süre (saniye) aşıldı. SNTP Istemcisi işlem sırasında devam eder, ancak SNTP sunucu durumu NX_FALSE olarak ayarlanır. Varsayılan değer 7200 ' dir.


**NX_SNTP_UPDATE_TIMEOUT_INTERVAL**  
SNTP Istemci süreölçerinin, son geçerli güncelleştirmeden bu yana kalan SNTP Istemci zamanını güncelleştirdiği zaman aralığı (saniye) ve tek noktaya yayın Istemcisi, sonraki SNTP güncelleştirme isteğini göndermeden önce kalan yoklama aralığı süresini güncelleştirir. Varsayılan değer 1’dir.

**NX_SNTP_CLIENT_UNICAST_POLL_INTERVAL**  
Istemcinin SNTP sunucusuna bir tek noktaya yayın isteği gönderdiği başlangıç yoklama aralığı (saniye). NetX Duo SNTP Istemci varsayılanı 3600 ' dir.

**NX_SNTP_CLIENT_EXP_BACKOFF_RATE**  
Geçerli Istemci tek noktaya yayın yoklama aralığının arttığı faktör. Istemci, bir sunucu saati güncelleştirmesi alamadığında veya sunucudan geçici olarak kullanılamayan (henüz eşitlenmemiş), zaman güncelleştirme hizmeti için geçerli yoklama aralığını arttıracaktır. bu hız, NX_SNTP_CLIENT_MAX_TIME_LAPSE aşmaz. Varsayılan değer 2 ' dir.

**NX_SNTP_CLIENT_RTT_REQUIRED**  
Etkinleştirilirse Bu seçenek, SNTP Istemcisinin, yerel saate sunucu güncelleştirmelerini uygularken SNTP iletilerinin gidiş dönüş süresini hesaplamasını gerektirir. Varsayılan değer NX_FALSE (devre dışı).

**NX_SNTP_CLIENT_MAX_ROOT_DISPERSION**  
Sunucu saati hassasiyetmesinin bir ölçüsü olan en fazla sunucu saati dağılımı (mikrosaniye), Istemci kabul eder. Bu gereksinimi devre dışı bırakmak için, en yüksek kök dağılımı için 0x0 olarak ayarlayın. NetX Duo SNTP Istemci varsayılanı 50000 olarak ayarlanmıştır.

**NX_SNTP_CLIENT_INVALID_UPDATE_LIMIT**  
Istemci sunucudan yayın veya tek noktaya yayın modunda alınan ardışık geçersiz güncelleştirme sayısı sınırı. Bu sınıra ulaşıldığında, Istemci geçerli SNTP sunucu durumunu geçersiz (NX_FALSE) olarak ayarlar, ancak sunucudan güncelleştirmeleri almaya çalışmaya devam edecektir. NetX Duo SNTP Istemci varsayılanı 3 ' dir.

**NX_SNTP_CLIENT_RANDOMIZE_ON_STARTUP**  
Bu, tek noktaya yayın modundaki SNTP Istemcisinin, rastgele bir bekleme aralığından sonra geçerli SNTP sunucusuyla ilk SNTP isteğini göndermesini gerekip gerekmediğini belirler. SNTP sunucusunda trafik tıkanıklığını sınırlamak için önemli sayıda SNTP Istemcisinin aynı anda başlatılmakta olduğu durumlarda kullanılır. Varsayılan değer NX_FALSE.

**NX_SNTP_CLIENT_SLEEP_INTERVAL**  
SNTP Istemci görevinin uyku moduna geçme zaman aralığı. Bu, uygulama API çağrılarının SNTP Istemcisi tarafından yürütülmesini sağlar. Varsayılan değer 1 Zamanlayıcı çentik ' dir.

**NX_SNTP_CURRENT_YEAR**  
Tarihi yıl/ay/tarih biçiminde göstermek için bu değeri geçerli yıldan eşit veya daha küçük olarak ayarlayın (değerlendirilmekte olan NTP süresi ile aynı yıl olması gerekir). Varsayılan değer 2015 ' dir.

**NTP_SECONDS_AT_01011999**  
Bu, ana NTP saatindeki ilk NTP dönemi için saniye cinsinden sayıdır. 0xBA368E80 olarak tanımlanmıştır. NTP saniyelik görüntülemeyi tarih ve saate devre dışı bırakmak için sıfır olarak ayarlayın.