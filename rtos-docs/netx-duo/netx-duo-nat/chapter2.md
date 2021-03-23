---
title: Bölüm 2-NAT yükleme ve kullanımı
description: Bu bölümde, NetX Duo NAT hizmetlerini yüklemek, ayarlamak ve kullanmak için bir açıklama yer almaktadır.
author: philmea
ms.author: philmea
ms.date: 07/14/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 47816c8a62aed9e2b096b121d1676c66178ad825
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104825864"
---
# <a name="chapter-2---installation-and-use-of-nat"></a>Bölüm 2-NAT yükleme ve kullanımı

Bu bölümde, NetX Duo NAT hizmetlerini yüklemek, ayarlamak ve kullanmak için bir açıklama yer almaktadır.

## <a name="netx-duo-nat-installation"></a>NetX Duo NAT yüklemesi

NetX Duo NAT, adresinde bulunabilir [https://github.com/azure-rtos/netxduo](https://github.com/azure-rtos/netxduo) . NetX Duo NAT paketi, bir kaynak dosyası ve bir üst bilgi dosyası, bir demo uygulama dosyası ve bu belge için bir PDF dosyası içerir ve aşağıdaki gibi:

- **nx_nat. c** NetX Duo NAT için C kaynak dosyası
- **nx_nat. h** NetX Duo NAT için C üstbilgi dosyası
- **demo_netx_nat. c** Örnek ana bilgisayar NetX Duo C kaynak dosyası
- **nx_nat.docx** NetX Duo NAT Kullanıcı kılavuzunun açıklaması (Bu belge)

NetX Duo NAT kaynak kodu dosyalarını, NetX Duo ve ThreadX 'in yüklü olduğu dizine kopyalayın. Örneğin, NetX Duo ve ThreadX "*\threadx\mcf5485\green*" dizinine yüklenirse, *nx_nat. c*, *Nx_nat. h ve değiştirilmiş NETX Duo dosyaları* bu dizine kopyalanmalıdır. Değiştirilmiş NetX Duo dosyalarını mevcut NetX Duo dosyaları üzerine kopyalayın. Ethernet Denetleyicisi sürücü dosyalarını da bu dizine kopyalayın.

NetX Duo NAT uygulaması oluşturmak için:

- NetX Duo Kitaplığı *nxduo. a* , tanımlı NX_NAT_ENABLED oluşturulmalıdır. Bu, *nx_user. h*' de yapılabilir ( *nx_user. h* içindeki yapılandırma seçeneklerinin derlemede yer aldığından emin olmak için NX_INCLUDE_USER_DEFINE_FILE de tanımlandığından emin olun.
- Uygulama Projesi, *tx_api. h* ve nx_api. h sonrasında *nx_nat. h* içermelidir. *Son iki başlık dosyası,* threadx ve NetX Duo hizmetlerini kullanmak için gereklidir.
- Uygulama daha sonra *nx_nat_enable* hizmetini kullanarak daha önce oluşturulmuş bir IP örneğinde NAT 'yi mümkün.
- Uygulama kodu, *nx_nat_enable* ve *NX_NAT_DISABLE* hizmetini çağırarak NAT 'ı dinamik olarak etkinleştirebilir/devre dışı bırakabilir.
- Uygulama proje kodu derlenir ve çalıştırılabilir dosyayı oluşturmak için NAT etkin NetX Duo kitaplığıyla bağlanır.
- TCP, UDP veya ıCMP protokollerini kullanarak NAT bağlantılarını desteklemek için, bu protokolü desteklemek üzere NetX Duo etkinleştirilmelidir. Bu, önceden oluşturulan IP örneği için *nx_tcp_enable, nx_udp_enable* ve *nx_icmp_enable* çağırarak yapılır.

## <a name="small-example-demo-nat-setup"></a>Küçük örnek Tanıtım NAT kurulumu

Uygulamanın NetX Duo NAT 'yi nasıl ayarladığını gösteren bir örnek, aşağıdaki Şekil 4 ' te *tx_application_define* işlevinde gösterilmiştir. Yükleme CD 'sinde dağıtılan NetX Duo tanıtım dosyalarından farklı olarak, bu tanıtım, *_nx_ram_network_driver*() sanal ağ sürücüsünü kullanan BIR Windows bilgisayarı yerine iki Ethernet denetleyicisi olan gerçek bir işlemci panosunda çalışır. NAT cihazı, yerel arabirimindeki yerel bir anahtar üzerinden yerel etki alanına ve dış arabirimindeki ikinci anahtar aracılığıyla dış ağa bağlanır.

NetXDuo temel yapılandırması demo_netx_nat. c içinde gösterilir. Özel ağ 192.168.2. xx olarak tanımlanır ve iki yerel konak düğümü vardır. Genel ağ, 192.168.0. xx olarak tanımlanır ve ağ geçidini 192.168.0.1 olarak ağ paketleri için tanımlar. NetX Duo IP örnekleri 118-171 satırları üzerinde oluşturulur ve ' RAM ' sürücüsünü çağırır; nat_ip örneği iliştirilmiş iki arabirim NAT local_ip yönlendiricisi olarak görev görür external_ip örneği eklenen bir arabirim dış konak olarak davranır.

NAT, satır 252 ' de oluşturulur ve dinamik çeviri girdilerini depolamak için önbelleği çağırır. Line319 ' de NAT özelliğini etkinleştirin, dış konağın yerel konağa erişmesine izin vermek için 362 satırlarında statik çeviri entrie (gelen girdisi) oluşturulur.

```C
/*
   demo_netx_nat.c

   This is a small demo of NAT (Network Address Translation) on the high-performance
   NetX TCP/IP stack.  This demo relies on ThreadX, NetX and NAT APIs to perform network
   address translation for IP packets traveling between private and external networks.
   this demo concentrates on the ICMP ping operation.
*/

#include   "tx_api.h"
#include   "nx_api.h"
#include   "nx_nat.h"

extern void    test_control_return(UINT status);
#if defined NX_NAT_ENABLE && defined __PRODUCT_NETXDUO__ && (NX_MAX_PHYSICAL_INTERFACES >= 2)

#define     DEMO_STACK_SIZE         2048

/* Define the ThreadX and NetX object control blocks...  */

static TX_THREAD                    ntest_0;

/* Set up the NAT components. */

/* Create a NAT instance, packet pool and translation table. */

NX_NAT_DEVICE                       nat_server;
NX_IP                               nat_ip;
NX_IP                               local_ip;
NX_IP                               external_ip;
NX_PACKET_POOL                      nat_packet_pool;
UINT                                error_counter = 0;


/* Configure the NAT network parameters. */

/* Set NetX IP packet pool packet size. This should be less than the Maximum Transmit Unit (MTU) of
   the driver (allow enough room for the Ethernet header plus padding bytes for frame alignment).  */
#define NX_NAT_PACKET_SIZE                          1536


/* Set the size of the NAT IP packet pool.  */
#define NX_NAT_PACKET_POOL_SIZE                     (NX_NAT_PACKET_SIZE * 10)

/* Set NetX IP helper thread stack size. */
#define NX_NAT_IP_THREAD_STACK_SIZE                 2048

/* Set the server IP thread priority */
#define NX_NAT_IP_THREAD_PRIORITY                   2

/* Set ARP cache size of a NAT ip instance. */
#define NX_NAT_ARP_CACHE_SIZE                       1024

/* Set NAT entries memory size. */
#define NX_NAT_ENTRY_CACHE_SIZE                     1024

/* Define NAT IP addresses, local host private IP addresses and external host IP address. */
#define NX_NAT_LOCAL_IPADR              (IP_ADDRESS(192, 168, 2, 1))
#define NX_NAT_LOCAL_HOST1              (IP_ADDRESS(192, 168, 2, 3))
#define NX_NAT_LOCAL_HOST2              (IP_ADDRESS(192, 168, 2, 10))
#define NX_NAT_LOCAL_GATEWAY            (IP_ADDRESS(192, 168, 2, 1))
#define NX_NAT_LOCAL_NETMASK            (IP_ADDRESS(255, 255, 255, 0))
#define NX_NAT_EXTERNAL_IPADR           (IP_ADDRESS(192, 168, 0, 10))
#define NX_NAT_EXTERNAL_HOST            (IP_ADDRESS(192, 168, 0, 100))
#define NX_NAT_EXTERNAL_GATEWAY         (IP_ADDRESS(192, 168, 0, 1))
#define NX_NAT_EXTERNAL_NETMASK         (IP_ADDRESS(255, 255, 255, 0))

/* Create NAT structures for creating NAT tables with static
   entries for local server hosts. */
NX_NAT_TRANSLATION_ENTRY            server_inbound_entry_icmp;

/* Define thread prototypes.  */
static void     ntest_0_entry(ULONG thread_input);
extern void    _nx_ram_network_driver(struct NX_IP_DRIVER_STRUCT *driver_req);

/* Define main entry point.  */

int main()
{

    /* Enter the ThreadX kernel.  */
    tx_kernel_enter();
}


/* Define what the initial system looks like.  */

void    tx_application_define(void *first_unused_memory)
{

    UINT     status;
    UCHAR    *pointer;

    /* Initialize the NetX system. */
    nx_system_initialize();

    /* Setup the pointer to unallocated memory.  */
    pointer =  (UCHAR *) first_unused_memory;

    /* Create the main thread.  */
    tx_thread_create(&ntest_0, "thread 0", ntest_0_entry, 0,
                     pointer, DEMO_STACK_SIZE,
                     4, 4, TX_NO_TIME_SLICE, TX_AUTO_START);
    pointer =  pointer + DEMO_STACK_SIZE;

    /* Create NAT packet pool. */
    status =  nx_packet_pool_create(&nat_packet_pool, "NAT Packet Pool",
                                    NX_NAT_PACKET_SIZE, pointer,
                                    NX_NAT_PACKET_POOL_SIZE);

    /* Update pointer to unallocated (free) memory. */
    pointer = pointer + NX_NAT_PACKET_POOL_SIZE;

    /* Check status.  */
    if (status)
        return;

    /* Create IP instances for NAT server (global network) */
    status = nx_ip_create(&nat_ip, "NAT IP Instance", NX_NAT_EXTERNAL_IPADR, NX_NAT_EXTERNAL_NETMASK,
                          &nat_packet_pool, _nx_ram_network_driver, pointer,
                          NX_NAT_IP_THREAD_STACK_SIZE, NX_NAT_IP_THREAD_PRIORITY);

    /* Update pointer to unallocated (free) memory. */
    pointer =  pointer + NX_NAT_IP_THREAD_STACK_SIZE;

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Set the private interface(private network).  */
    status += nx_ip_interface_attach(&nat_ip, "Private Interface", NX_NAT_LOCAL_IPADR,
        NX_NAT_LOCAL_NETMASK, _nx_ram_network_driver);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Create IP instances for Local network IP instance */
    status = nx_ip_create(&local_ip, "Local IP Instance", NX_NAT_LOCAL_HOST1, NX_NAT_LOCAL_NETMASK,
                          &nat_packet_pool, _nx_ram_network_driver, pointer,
                          NX_NAT_IP_THREAD_STACK_SIZE, NX_NAT_IP_THREAD_PRIORITY);

    /* Update pointer to unallocated (free) memory. */
    pointer =  pointer + NX_NAT_IP_THREAD_STACK_SIZE;

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Create IP instances for external network IP instance */
    status = nx_ip_create(&external_ip, "External IP Instance", NX_NAT_EXTERNAL_HOST,
                        NX_NAT_EXTERNAL_NETMASK,
                        &nat_packet_pool, _nx_ram_network_driver, pointer,
                        NX_NAT_IP_THREAD_STACK_SIZE, NX_NAT_IP_THREAD_PRIORITY);

    /* Update pointer to unallocated (free) memory. */
    pointer =  pointer + NX_NAT_IP_THREAD_STACK_SIZE;

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Set the global network gateway for NAT IP instance.  */
    status = nx_ip_gateway_address_set(&nat_ip, NX_NAT_EXTERNAL_GATEWAY);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Set the global network gateway for Local IP instance.  */
    status = nx_ip_gateway_address_set(&local_ip, NX_NAT_LOCAL_GATEWAY);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Set the global network gateway for External IP instance.  */
    status = nx_ip_gateway_address_set(&external_ip, NX_NAT_EXTERNAL_GATEWAY);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }


    /* Enable ARP and supply ARP cache memory for NAT IP isntance. */
    status =  nx_arp_enable(&nat_ip, (void **) pointer,
                            NX_NAT_ARP_CACHE_SIZE);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Update pointer to unallocated (free) memory. */
    pointer = pointer + NX_NAT_ARP_CACHE_SIZE;

    /* Enable ARP and supply ARP cache memory for Local IP isntance. */
    status =  nx_arp_enable(&local_ip, (void **) pointer,
                            NX_NAT_ARP_CACHE_SIZE);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Update pointer to unallocated (free) memory. */
    pointer = pointer + NX_NAT_ARP_CACHE_SIZE;

    /* Enable ARP and supply ARP cache memory for External IP isntance. */
    status =  nx_arp_enable(&external_ip, (void **) pointer,
                            NX_NAT_ARP_CACHE_SIZE);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Update pointer to unallocated (free) memory. */
    pointer = pointer + NX_NAT_ARP_CACHE_SIZE;

    /* Enable ICMP. */
    nx_icmp_enable(&nat_ip);
    nx_icmp_enable(&local_ip);
    nx_icmp_enable(&external_ip);

    /* Create a NetX NAT server and cache with a global interface index.  */
    status =  nx_nat_create(&nat_server, &nat_ip, 0, pointer, NX_NAT_ENTRY_CACHE_SIZE);

    /* Check status.  */
    if (status)
    {
        error_counter++;
        return;
    }

    /* Update pointer to unallocated (free) memory. */
    pointer = pointer + NX_NAT_ENTRY_CACHE_SIZE;
}

/* Define the test threads.  */

static void    ntest_0_entry(ULONG thread_input)
{

UINT        status;
NX_PACKET   *my_packet;

    /***********************************/
    /*       Disable NAT feature       */
    /***********************************/
    /* Local Host ping External Host address.  */
    status =  nx_icmp_ping(&local_ip, NX_NAT_EXTERNAL_HOST,
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ", 28, &my_packet, 100);

    /* Check status.  */
    if (status == NX_SUCCESS)
    {
        error_counter++;
        return;
    }

    /* Check the NAT forwarded count.  */
#ifndef NX_DISABLE_NAT_INFO
    if ((nat_server.forwarded_packets_received != 0) ||
        (nat_server.forwarded_packets_sent != 0) ||
        (nat_server.arded_packets_dropped != 0))
    {
        error_counter++;
        return;
    }
#endif

    /* External Host ping NAT External address, NAT IP instance will response the requet.  */
    status = nx_icmp_ping(&external_ip, NX_NAT_EXTERNAL_IPADR,
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ", 28, &my_packet, 100);

    /* Check status.  */
    if ((status != NX_SUCCESS) || (my_packet == NX_NULL) || (my_packet -> nx_packet_length != 28))
    {
        error_counter++;
        return;

    /* Check the NAT forwarded count.  */
#ifndef NX_DISABLE_NAT_INFO
    if ((nat_server.forwarded_packets_received != 0) ||
        (nat_server.forwarded_packets_sent != 0) ||
        (nat_server.arded_packets_dropped != 0))
    {
        error_counter++;
        return;
    }
#endif
    }

    /***********************************/
    /*       Enable NAT feature        */
    /***********************************/

    /* Enable the NAT service.  */
    nx_nat_enable(&nat_server);

    /* Local Host ping External Host address.  */
    status =  nx_icmp_ping(&local_ip, NX_NAT_EXTERNAL_HOST,
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ", 28, &my_packet, 100);

    if ((status != NX_SUCCESS) || (my_packet == NX_NULL) || (my_packet -> nx_packet_length != 28))
    {
        error_counter++;
        return;
    }

    /* Check the NAT forwarded count.  */
#ifndef NX_DISABLE_NAT_INFO
    if ((nat_server.forwarded_packets_received != 2) ||
        (nat_server.forwarded_packets_sent != 2) ||
        (nat_server.arded_packets_dropped != 0))
    {
        error_counter++;
        return;
    }
#endif

    /* External Host ping NAT External address, NAT IP instance will response the requet.  */
    status =  nx_icmp_ping(&external_ip, NX_NAT_EXTERNAL_IPADR,
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ", 28, &my_packet, 100);

    if ((status != NX_SUCCESS) || (my_packet == NX_NULL) || (my_packet -> nx_packet_length != 28))
    {
        error_counter++;
        return;
    }

    /* Check the NAT forwarded count.  NAT receive the ping request,
        but can not forward this packet to local network.  discard it.  
#ifndef NX_DISABLE_NAT_INFO
    if ((nat_server.forwarded_packets_received != 3) ||
        (nat_server.forwarded_packets_sent != 2) ||
        (nat_server.arded_packets_dropped != 1))
    {
        error_counter++;
        return;
    }
#endif

    /**********************************************/
    /*       Create an inbound entry for ICMP     */
    /**********************************************/

    /* Calling NAT API to create a inbound entry.  */
    status = nx_nat_inbound_entry_create(&nat_server, &server_inbound_entry_icmp,
        NX_NAT_LOCAL_HOST1, 0, 0, NX_PROTOCOL_ICMP);

    if (status != NX_SUCCESS)
    {
        error_counter++;
        return;
    }

    /* External Host ping NAT External address, LOCAL HOST1 will
        response all inbound icmp request from external network.  */
    status =  nx_icmp_ping(&external_ip, NX_NAT_EXTERNAL_IPADR,
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ", 28, &my_packet, 100);

    if ((status != NX_SUCCESS) || (my_packet == NX_NULL) || (my_packet -> nx_packet_length != 28))
    {
        error_counter++;
        return;
    }

    /* Check the NAT forwarded count.  */
#ifndef NX_DISABLE_NAT_INFO
    if ((nat_server.forwarded_packets_received != 5) ||
        (nat_server.forwarded_packets_sent != 4) ||
        (nat_server.arded_packets_dropped != 1))
    {
        error_counter++;
        return;
    }
#endif
}
#endif
```

**Şekil 5-NetX Duo NAT 'yi ayarlama**