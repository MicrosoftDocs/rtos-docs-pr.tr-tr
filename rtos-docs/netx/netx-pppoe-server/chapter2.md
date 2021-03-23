---
title: Bölüm 2-Azure RTOS NetX PPPoE sunucusunu yükleme ve kullanma
description: Bu bölümde, Azure RTOS NetX PPPoE sunucu bileşeninin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.
author: philmea
ms.author: philmea
ms.date: 06/04/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 5b52164911676b68c67da01d698e41c02730e45a
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104825588"
---
# <a name="chapter-2---installation-and-use-of-azure-rtos-netx-pppoe-server"></a><span data-ttu-id="bd9ff-103">Bölüm 2-Azure RTOS NetX PPPoE sunucusunu yükleme ve kullanma</span><span class="sxs-lookup"><span data-stu-id="bd9ff-103">Chapter 2 - Installation and use of Azure RTOS NetX PPPoE Server</span></span>

<span data-ttu-id="bd9ff-104">Bu bölümde, Azure RTOS NetX PPPoE sunucu bileşeninin yüklenmesi, kurulumu ve kullanımı ile ilgili çeşitli sorunların bir açıklaması yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-104">This chapter contains a description of various issues related to installation, setup, and usage of the Azure RTOS NetX PPPoE Server component.</span></span>

## <a name="product-distribution"></a><span data-ttu-id="bd9ff-105">Ürün dağıtımı</span><span class="sxs-lookup"><span data-stu-id="bd9ff-105">Product Distribution</span></span>

<span data-ttu-id="bd9ff-106">NetX için PPPoE sunucusu, adresinde bulunabilir [https://github.com/azure-rtos/netx](https://github.com/azure-rtos/netx) .</span><span class="sxs-lookup"><span data-stu-id="bd9ff-106">PPPoE Server for NetX is available at [https://github.com/azure-rtos/netx](https://github.com/azure-rtos/netx).</span></span> <span data-ttu-id="bd9ff-107">Paket, aşağıdaki gibi, bu belgeyi içeren iki kaynak dosya ve bir PDF dosyası içerir:</span><span class="sxs-lookup"><span data-stu-id="bd9ff-107">The package includes two source files and a PDF file that contains this document, as follows:</span></span>

- <span data-ttu-id="bd9ff-108">**nx_pppoe_server. h**: NETX Için PPPoE sunucusu için üst bilgi dosyası</span><span class="sxs-lookup"><span data-stu-id="bd9ff-108">**nx_pppoe_server.h**: Header file for PPPoE Server for NetX</span></span>
- <span data-ttu-id="bd9ff-109">**nx_pppoe_server. c**: NETX Için PPPoE sunucusu Için c kaynak dosyası</span><span class="sxs-lookup"><span data-stu-id="bd9ff-109">**nx_pppoe_server.c**: C Source file for PPPoE Server for NetX</span></span>
- <span data-ttu-id="bd9ff-110">**nx_pppoe_server.pdf**: NETX Için PPPoE sunucusunun PDF açıklaması</span><span class="sxs-lookup"><span data-stu-id="bd9ff-110">**nx_pppoe_server.pdf**: PDF description of PPPoE Server for NetX</span></span>
- <span data-ttu-id="bd9ff-111">**demo_netx_pppoe_server. c**: NETX PPPoE sunucu tanıtımı</span><span class="sxs-lookup"><span data-stu-id="bd9ff-111">**demo_netx_pppoe_server.c**: NetX PPPoE Server demonstration</span></span>

## <a name="pppoe-server-installation"></a><span data-ttu-id="bd9ff-112">PPPoE sunucu yüklemesi</span><span class="sxs-lookup"><span data-stu-id="bd9ff-112">PPPoE Server Installation</span></span>

<span data-ttu-id="bd9ff-113">NetX için PPPoE sunucusunu kullanabilmeniz için, daha önce bahsedilen dağıtımın tamamı, NetX 'in yüklü olduğu dizine kopyalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-113">In order to use PPPoE Server for NetX, the entire distribution mentioned previously should be copied to the same directory where NetX is installed.</span></span> <span data-ttu-id="bd9ff-114">Örneğin, "*\threadx\arm7\green*" dizininde NETX yüklüyse, *nx_pppoe_server. h* ve *nx_pppoe_server. c* dosyaları bu dizine kopyalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-114">For example, if NetX is installed in the directory "*\threadx\arm7\green*" then the *nx_pppoe_server.h* and *nx_pppoe_server.c* files should be copied into this directory.</span></span>

## <a name="using-pppoe-server"></a><span data-ttu-id="bd9ff-115">PPPoE sunucusunu kullanma</span><span class="sxs-lookup"><span data-stu-id="bd9ff-115">Using PPPoE Server</span></span>

<span data-ttu-id="bd9ff-116">NetX için PPPoE sunucusu kullanmak kolaydır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-116">Using PPPoE Server for NetX is easy.</span></span> <span data-ttu-id="bd9ff-117">Temel olarak, uygulama kodu sırasıyla ThreadX ve NetX kullanmak için *tx_api. h* ve *nx_api. h* dahil *nx_pppoe_server.* h içermelidir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-117">Basically, the application code must include *nx_pppoe_server.h* after it includes *tx_api.h* and *nx_api.h*, in order to use ThreadX and NetX, respectively.</span></span> <span data-ttu-id="bd9ff-118">*Nx_pppoe_server. h* eklendikten sonra, uygulama kodu bu kılavuzda daha sonra belirtilen PPPoE sunucu işlev çağrılarını yapabilir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-118">Once *nx_pppoe_server.h* is included, the application code is then able to make the PPPoE Server function calls specified later in this guide.</span></span> <span data-ttu-id="bd9ff-119">Uygulama, yapı işlemine *nx_pppoe_server. c* de içermelidir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-119">The application must also include *nx_pppoe_server.c* in the build process.</span></span> <span data-ttu-id="bd9ff-120">Bu dosya, diğer uygulama dosyalarıyla aynı şekilde derlenmelidir ve nesne formu, uygulamanın dosyalarıyla birlikte bağlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-120">This file must be compiled in the same manner as other application files and its object form must be linked along with the files of the application.</span></span> <span data-ttu-id="bd9ff-121">Bu, NetX PPPoE sunucusunu kullanmak için gereklidir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-121">This is all that is required to use NetX PPPoE Server.</span></span>

## <a name="small-example-system"></a><span data-ttu-id="bd9ff-122">Küçük örnek sistem</span><span class="sxs-lookup"><span data-stu-id="bd9ff-122">Small Example System</span></span>

<span data-ttu-id="bd9ff-123">Aşağıda, The NetX PPPoE sunucusunun nasıl kullanıldığını gösteren bir örnek verilmiştir. Şekil 1,1.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-123">The following is an example that illustrates how to use NetX PPPoE Server is described in Figure 1.1.</span></span> <span data-ttu-id="bd9ff-124">Bu örnekte, PPPoE sunucusu içerme dosyası *nx_pppoe_server. h* , 50. satırda getirilir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-124">In this example, the PPPoE Server include file *nx_pppoe_server.h* is brought in at line 50.</span></span> <span data-ttu-id="bd9ff-125">Ardından, PPPoE sunucusu 248 satırındaki *"thread_0_entry*" içinde oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-125">Next, PPPoE Server is created in *"thread_0_entry*" at line 248.</span></span> <span data-ttu-id="bd9ff-126">IP örneği oluşturulduktan sonra PPPoE sunucusunun oluşturulması gerektiğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-126">Note that PPPoE Server should be created after create the IP instance.</span></span> <span data-ttu-id="bd9ff-127">IP örneği oluşturulur ve line165 başlatılır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-127">The IP instance is created and initialized line165.</span></span> <span data-ttu-id="bd9ff-128">"*Pppoe_server*" PPPoE sunucu denetim bloğu, daha önce satır 79 ' de genel bir değişken olarak tanımlandı.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-128">The PPPoE Server control block "*pppoe_server*" was defined as a global variable at line 79 previously.</span></span> <span data-ttu-id="bd9ff-129">Bildirim işlevleri, satır 257 ' de ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-129">The notify functions are set at line 257.</span></span> <span data-ttu-id="bd9ff-130">Pppoe_session_data_receive bildirme işlevinin ayarlanmış olması gerektiğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-130">Note that pppoe_session_data_receive notify function must be set.</span></span> <span data-ttu-id="bd9ff-131">IP ve PPPoE sunucusu başarıyla oluşturulduktan sonra, PPPoE sunucusu, 272 satırındaki nx_pppoe_server_enable çağrısında bir PPPoE oturumu oluşturma işlemidir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-131">After successful creation of IP and PPPoE Server, the PPPoE Server process of establishing a PPPoE session at the call to nx_pppoe_server_enable at line 272.</span></span>

<span data-ttu-id="bd9ff-132">Genel olarak, PPPoE modülünün PPP modülüyle birlikte kullanılması gerekir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-132">In general, PPPoE module should be used with PPP module.</span></span> <span data-ttu-id="bd9ff-133">Bu örnekte, PPP sunucusu içerme dosyası *nx_ppp. h* , 49. satırda getirilir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-133">In this example, the PPP Server include file *nx_ppp.h* is brought in at line 49.</span></span> <span data-ttu-id="bd9ff-134">Daha sonra, 174 satırındaki PPP sunucusu oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-134">Next, PPP Server is created at line 174.</span></span> <span data-ttu-id="bd9ff-135">Satır 182 PPP paketini göndermek için işlevi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-135">Line 182 setup the function to send PPP packet.</span></span> <span data-ttu-id="bd9ff-136">Satır 188-200 IP adreslerini ayarlayın ve PAP protokolünü tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-136">Line 188-200 setup the IP addresses and define the pap protocol.</span></span> <span data-ttu-id="bd9ff-137">Satır 115-139 PAP protokolü için Kullanıcı adı ve parola ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-137">Line 115-139 setup the user name and password for pap protocol.</span></span>

<span data-ttu-id="bd9ff-138">PPPoE oturumu kurulduktan sonra.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-138">After the PPPoE session established.</span></span> <span data-ttu-id="bd9ff-139">Uygulama, 281 satırındaki oturum bilgilerini (istemci MAC adresi ve oturum kimliği) almak için nx_pppoe_server_session_get çağırabilir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-139">The application can call nx_pppoe_server_session_get to get the session information (client MAC address and session id) at line 281.</span></span>

<span data-ttu-id="bd9ff-140">Uygulama artık PPP trafiğini işlememesi durumunda, uygulama PppCloseInd veya nx_pppoe_server_session_terminate ve PPPoE oturumunu sonlandırır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-140">When the application no longer process PPP traffic, the application PppCloseInd or nx_pppoe_server_session_terminate to terminate the PPPoE session.</span></span>

> [!NOTE]
> <span data-ttu-id="bd9ff-141">Bu örnekte, PPPoE sunucusu normal IP Stack ile aynı anda çalışır ve bir Ethernet sürücüsünü paylaşır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-141">In this example, PPPoE Server work with normal IP stack at the same time, and share one Ethernet driver.</span></span> <span data-ttu-id="bd9ff-142">Normal IP örneği için aynı Ethernet sürücüsünü, 165. satırda ve PPPoE sunucu 248 örneğine geçirin.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-142">Pass the same Ethernet driver for normal IP instance at line 165 and PPPoE Server instance at line 248.</span></span>

> [!NOTE]
> <span data-ttu-id="bd9ff-143">İşlevler, tanımlanan NX_PPPoE_SERVER_SESSION_CONTROL_ENABELE altında yazılım tarafından çağrılması için PPPoE uygulamasıyla sağlanır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-143">The functions are provided by the PPPoE implementation for calling by the software under defined NX_PPPoE_SERVER_SESSION_CONTROL_ENABELE.</span></span>

<span data-ttu-id="bd9ff-144">Tanımlanmışsa, PPPoE oturumunu denetleyen özelliği sunar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-144">If defined, enables the feature that controls the PPPoE session.</span></span>

<span data-ttu-id="bd9ff-145">Uygulama belirli API 'yi çağırana kadar, PPPoE sunucusu isteğe otomatik olarak yanıt vermez, PPPoE sunucusu isteğe otomatik olarak yanıt vermez.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-145">PPPoE server does not automatically response to the request until application call specific API, if not defined, PPPoE Server automatically responses to the request.</span></span> <span data-ttu-id="bd9ff-146">Nx_pppoe_server. h içinde varsayılan olarak etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-146">It enables by default in nx_pppoe_server.h.</span></span>

<span data-ttu-id="bd9ff-147">Fiziksel üstbilgiyi doldurmak için yeterli alan olduğundan emin olmak için **NX_PHYSICAL_HEADER** 24 ' e yeniden tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-147">Note, redefine **NX_PHYSICAL_HEADER** to 24 to ensure enough space for filling in physical header.</span></span> <span data-ttu-id="bd9ff-148">Fiziksel üst bilgi: 14 (Ethernet üstbilgisi) + 6 (PPPoE üstbilgisi) + 2 (PPP üstbilgisi) + 2 (dört baytlık bir Aligment).</span><span class="sxs-lookup"><span data-stu-id="bd9ff-148">Physical header:14(Ethernet header) + 6(PPPoE header) + 2(PPP header) + 2(four-byte aligment).</span></span>

```c
/**************************************************************************/
/**************************************************************************/
/**                                                                       */
/** NetX PPPoE Server stack Component                                     */
/**                                                                       */
/** This is a small demo of the high-performance NetX PPPoE Server        */
/** stack. This demo includes IP instance, PPPoE Server and PPP Server    */
/** stack. Create one IP instance includes two interfaces to support      */
/** for normal IP stack and PPPoE Server, PPPoE Server can use the        */
/** mutex of IP instance to send PPPoE message when share one Ethernet    */
/** driver. PPPoE Server work with normal IP instance at the same time.   */
/**                                                                       */
/** Note1: Substitute your Ethernet driver instead of                     */
/** _nx_ram_network_driver before run this demo                           */
/**                                                                       */
/** Note2: Prerequisite for using PPPoE.                                  */
/** Redefine NX_PHYSICAL_HEADER to 24 to ensure enough space for filling  */
/** in physical header. Physical header:14(Ethernet header)               */
/** + 6(PPPoE header) + 2(PPP header) + 2(four-byte aligment)             */
/**                                                                       */
/**************************************************************************/
/**************************************************************************/


/*****************************************************************/
/*                            NetX Stack                         */
/*****************************************************************/

                                      /***************************/
                                      /* PPP Server              */
                                      /***************************/

                                      /***************************/
                                      /* PPPoE Server            */
                                      /***************************/
/***************************/         /***************************/
/* Normal Ethernet Type    */         /* PPPoE Ethernet Type     */
/***************************/         /***************************/
/***************************/         /***************************/
/* Interface 0             */         /* Interface 1             */
/***************************/         /***************************/

/*****************************************************************/
/*                     Ethernet Dirver                           */
/*****************************************************************/

#include     "tx_api.h"
#include     "nx_api.h"
#include     "nx_ppp.h"
#include     "nx_pppoe_server.h"

/* Defined NX_PPP_PPPOE_ENABLE if use Express Logic's PPP, since PPP module has been modified to match PPPoE moduler under this definition. */
#ifdef NX_PPP_PPPOE_ENABLE

/*   If the driver is not initialized in other module, define */
/*   NX_PPPOE_SERVER_INITIALIZE_DRIVER_ENABLE to initialize the driver in PPPoE module. */
/*   In this demo, the driver has been initialized in IP module. */

#ifdef NX_PPPOE_SERVER_INITIALIZE_DRIVER_ENABLE

/*   NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE: If defined, enables the feature that */
/*   controls the PPPoE session. PPPoE server does not automatically response to the */
/*   request until application call specific API. */

/* Define the block size. */
#define     NX_PACKET_POOL_SIZE     ((1536 + sizeof(NX_PACKET)) * 30)
#define     DEMO_STACK_SIZE         2048
#define     PPPOE_THREAD_SIZE       2048

/* Define the ThreadX and NetX object control blocks... */
TX_THREAD           thread_0;

/* Define the packet pool and IP instance for normal IP instnace. */
NX_PACKET_POOL      pool_0;
NX_IP               ip_0;

/* Define the PPP Server instance. */
NX_PPP              ppp_server;

/* Define the PPPoE Server instance. */
NX_PPPOE_SERVER     pppoe_server;

/* Define the counters. */
CHAR                *pointer;
ULONG               error_counter;

/* Define thread prototypes. */
void     thread_0_entry(ULONG thread_input);

/***** Substitute your PPP driver entry function here *********/
extern void     _nx_ppp_driver(NX_IP_DRIVER *driver_req_ptr);

/***** Substitute your Ethernet driver entry function here *********/
extern void     _nx_ram_network_driver(NX_IP_DRIVER *driver_req_ptr);

/* Define the callback functions. */
void     PppDiscoverReq(UINT interfaceHandle);
void     PppOpenReq(UINT interfaceHandle, ULONG length, UCHAR *data);
void     PppCloseRsp(UINT interfaceHandle);
void     PppCloseReq(UINT interfaceHandle);
void     PppTransmitDataReq(UINT interfaceHandle, ULONG length, UCHAR *data, UINT packet_id);
void     PppReceiveDataRsp(UINT interfaceHandle, UCHAR *data);

/* Define the porting layer function for Express Logic's PPP to simulate TTP's PPP. */
/* Functions to be provided by PPP for calling by the PPPoE Stack. */
void     ppp_server_packet_send(NX_PACKET *packet_ptr);

/* Define main entry point. */

int main()
{

    /* Enter the ThreadX kernel. */
    tx_kernel_enter();
}

UINT verify_login(CHAR *name, CHAR *password)
{

    if ((name[0] == 'm') &&
        (name[1] == 'y') &&
        (name[2] == 'n') &&
        (name[3] == 'a') &&
        (name[4] == 'm') &&
        (name[5] == 'e') &&
        (name[6] == (CHAR) 0) &&
        (password[0] == 'm') &&
        (password[1] == 'y') &&
        (password[2] == 'p') &&
        (password[3] == 'a') &&
        (password[4] == 's') &&
        (password[5] == 's') &&
        (password[6] == 'w') &&
        (password[7] == 'o') &&
        (password[8] == 'r') &&
        (password[9] == 'd') &&
        (password[10] == (CHAR) 0))
            return(NX_SUCCESS);
    else
        return(NX_PPP_ERROR);
}

/* Define what the initial system looks like. */

void tx_application_define(void *first_unused_memory)
{

    UINT status;

    /* Setup the working pointer. */
    pointer = (CHAR *) first_unused_memory;

    /* Initialize the NetX system. */
    nx_system_initialize();

    /* Create a packet pool for normal IP instance. */
    status = nx_packet_pool_create(&pool_0, "NetX Main Packet Pool",
                                    (1536 + sizeof(NX_PACKET)),
                                    pointer, NX_PACKET_POOL_SIZE);
                                    pointer = pointer + NX_PACKET_POOL_SIZE;

    /* Check for error. */
    if (status)
        error_counter++;

    /* Create an normal IP instance. */
    status = nx_ip_create(&ip_0, "NetX IP Instance", IP_ADDRESS(192, 168, 100, 43),
                        0xFFFFFF00UL, &pool_0, _nx_ram_network_driver,
                        pointer, 2048, 1);
                        pointer = pointer + 2048;

    /* Check for error. */
    if (status)
        error_counter++;

    /* Create the PPP instance. */
    status = nx_ppp_create(&ppp_server, "PPP Instance", &ip_0, pointer, 2048, 1,
                            &pool_0, NX_NULL, NX_NULL);
    pointer = pointer + 2048;

    /* Check for PPP create error. */
    if (status)
        error_counter++;

    /* Set the PPP packet send function. */
    status = nx_ppp_packet_send_set(&ppp_server, ppp_server_packet_send);

    /* Check for PPP packet send function set error. */
    if (status)
        error_counter++;

    /* Define IP address. This PPP instance is effectively the server since it has both IP addresses. */
    status = nx_ppp_ip_address_assign(&ppp_server, IP_ADDRESS(192, 168, 10, 43),                                         IP_ADDRESS(192, 168, 10, 44));

    /* Check for PPP IP address assign error. */
    if (status)
        error_counter++;

    /* Setup PAP, this PPP instance is effectively the server since it will verify the name and password. */
    status = nx_ppp_pap_enable(&ppp_server, NX_NULL, verify_login);

    /* Check for PPP PAP enable error. */
    if (status)
        error_counter++;

    /* Attach an interface for PPP. */
    status = nx_ip_interface_attach(&ip_0, "Second Interface For PPP", 
                            IP_ADDRESS(0, 0, 0, 0), 0, nx_ppp_driver);

    /* Check for error. */
    if (status)
        error_counter++;

    /* Enable ARP and supply ARP cache memory for Normal IP Instance. */
    status = nx_arp_enable(&ip_0, (void *) pointer, 1024);
    pointer = pointer + 1024;

    /* Check for ARP enable errors. */
    if (status)
        error_counter++;

    /* Enable ICMP */
    status = nx_icmp_enable(&ip_0);
    if(status)
        error_counter++;

    /* Enable UDP traffic. */
    status = nx_udp_enable(&ip_0);
    if (status)
        error_counter++;

    /* Enable TCP traffic. */
    status = nx_tcp_enable(&ip_0);
    if (status)
        error_counter++;

    /* Create the main thread. */
    tx_thread_create(&thread_0, "thread 0", thread_0_entry, 0,
                    pointer, DEMO_STACK_SIZE,
                    4, 4, TX_NO_TIME_SLICE, TX_AUTO_START);
                    pointer = pointer + DEMO_STACK_SIZE;
}

/* Define the test threads. */

void     thread_0_entry(ULONG thread_input)
{
UINT     status;
ULONG    ip_status;

    /* Create the PPPoE instance. */
    status = nx_pppoe_server_create(&pppoe_server, (UCHAR *)"PPPoE Server", &ip_0, 0,
                    _nx_ram_network_driver, &pool_0, pointer, PPPOE_THREAD_SIZE, 4);
    pointer = pointer + PPPOE_THREAD_SIZE;
    if (status)
    {
        error_counter++;
        return;
    }

    /* Set the callback notify function. */
    status = nx_pppoe_server_callback_notify_set(&pppoe_server, PppDiscoverReq,
        PppOpenReq, PppCloseRsp, PppCloseReq, PppTransmitDataReq, PppReceiveDataRsp);

    if (status)
    {
        error_counter++;
        return;
    }

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call function function to set the default service Name. */
        /* PppInitInd(length, aData); */
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */

    /* Enable PPPoE Server. */
    status = nx_pppoe_server_enable(&pppoe_server);
    if (status)
    {
        error_counter++;
        return;
    }

    /* Get the PPPoE Client physical address and Session ID after establish PPPoE Session. */
    /*
        status = nx_pppoe_server_session_get(&pppoe_server, interfaceHandle, &client_mac_msw, &client_mac_lsw, &session_id);
        if (status)
            error_counter++;
    */

    /* Wait for the link to come up. */
    status = nx_ip_interface_status_check(&ip_0, 1, NX_IP_ADDRESS_RESOLVED,
                                            &ip_status, NX_WAIT_FOREVER);
    if (status)
    {
        error_counter++;
        return;
    }

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call PPPoE function to terminate the PPPoE Session. */
        /* PppCloseInd(interfaceHandle, causeCode); */
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */

}

void     PppDiscoverReq(UINT interfaceHandle)
{

    /* Receive the PPPoE Discovery Initiation Message. */
    
    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call PPPoE function to allow TTP's software to define the Service Name field of the PADO packet. */
        PppDiscoverCnf(0, NX_NULL, interfaceHandle);
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */
}

void     PppOpenReq(UINT interfaceHandle, ULONG length, UCHAR *data)
{

    /* Get the notify that receive the PPPoE Discovery Request Message. */

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call PPPoE function to allow TTP's software to accept the PPPoE session. */
        PppOpenCnf(NX_TRUE, interfaceHandle);
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */
}

void     PppCloseRsp(UINT interfaceHandle)
{

    /* Get the notify that receive the PPPoE Discovery Terminate Message. */

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call PPPoE function to allow TTP's software to confirm that the handle has been freed. */
        PppCloseCnf(interfaceHandle);
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */
}

void     PppCloseReq(UINT interfaceHandle)
{

    /* Get the notify that PPPoE Discovery Terminate Message has been sent. */

}

void     PppTransmitDataReq(UINT interfaceHandle, ULONG length, UCHAR *data, UINT packet_id)
{

    NX_PACKET *packet_ptr;

    /* Get the notify that receive the PPPoE Session data. */

    /* Call PPP Server to receive the PPP data fame. */
    packet_ptr = (NX_PACKET *)(packet_id);
    nx_ppp_packet_receive(&ppp_server, packet_ptr);

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        /* Call PPPoE function to confirm that the data has been processed. */
        PppTransmitDataCnf(interfaceHandle, data, packet_id);
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */
}

void     PppReceiveDataRsp(UINT interfaceHandle, UCHAR *data)
{

    /* Get the notify that the PPPoE Session data has been sent. */

}

/* PPP Server send function. */
void     ppp_server_packet_send(NX_PACKET *packet_ptr)
{

    /* For Express Logic's PPP test, the session should be the first session, so set interfaceHandle as 0. */
    UINT interfaceHandle = 0;

    #ifdef NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE
        while(packet_ptr)
        {

            /* Call functions to be provided by PPPoE for TTP. */
            PppReceiveDataInd(interfaceHandle, (packet_ptr -> nx_packet_append_ptr -
            packet_ptr -> nx_packet_prepend_ptr), packet_ptr -> nx_packet_prepend_ptr);

            /* Move to the next packet structure. */
            packet_ptr = packet_ptr -> nx_packet_next;
        }
    #else
        /* Directly Call PPPoE send function to send out the data through PPPoE module. */
        nx_pppoe_server_session_packet_send(&pppoe_server, interfaceHandle, packet_ptr);
    #endif /* NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE */
}
#endif /* NX_PPPOE_SERVER_INITIALIZE_DRIVER_ENABLE */

#endif /* NX_PPP_PPPOE_ENABLE */
```

<span data-ttu-id="bd9ff-149">Şekil 1,1 NetX ile PPPoE sunucu kullanımı örneği</span><span class="sxs-lookup"><span data-stu-id="bd9ff-149">Figure 1.1 Example of PPPoE Server use with NetX</span></span>

## <a name="configuration-options"></a><span data-ttu-id="bd9ff-150">Yapılandırma seçenekleri</span><span class="sxs-lookup"><span data-stu-id="bd9ff-150">Configuration Options</span></span>

<span data-ttu-id="bd9ff-151">NetX için PPPoE sunucusu oluşturmaya yönelik birkaç yapılandırma seçeneği vardır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-151">There are several configuration options for building PPPoE Server for NetX.</span></span> <span data-ttu-id="bd9ff-152">Aşağıdaki listede her biri ayrıntılı açıklanmıştır:</span><span class="sxs-lookup"><span data-stu-id="bd9ff-152">The following list describes each in detail:</span></span>

- <span data-ttu-id="bd9ff-153">**NX_DISABLE_ERROR_CHECKING**: tanımlı, bu seçenek temel PPPoE sunucusu hata denetimini kaldırır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-153">**NX_DISABLE_ERROR_CHECKING**: Defined, this option removes the basic PPPoE Server error checking.</span></span> <span data-ttu-id="bd9ff-154">Genellikle uygulamanın hata ayıklaması yapıldıktan sonra kullanılır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-154">It is typically used after the application has been debugged.</span></span>

- <span data-ttu-id="bd9ff-155">**NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE**: tanımlanmışsa, PPPoE oturumunu denetleyen özelliği sunar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-155">**NX_PPPOE_SERVER_SESSION_CONTROL_ENABLE**: If defined, enables the feature that controls the PPPoE session.</span></span> <span data-ttu-id="bd9ff-156">PPPoE sunucusu, uygulama belirli bir API 'YI çağırana kadar isteğe otomatik olarak yanıt vermez.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-156">PPPoE server does not automatically response to the request until application call specific API.</span></span>

- <span data-ttu-id="bd9ff-157">**NX_PPPOE_SERVER_INITIALIZE_DRIVER_ENABLE**: tanımlanmışsa, özelliğin PPPoE modülünde Ethernet sürücüsünü başlatmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-157">**NX_PPPOE_SERVER_INITIALIZE_DRIVER_ENABLE**: If defined, enables the feature to initialize the Ethernet driver in PPPoE module.</span></span> <span data-ttu-id="bd9ff-158">Varsayılan olarak devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-158">It disables by default.</span></span>

- <span data-ttu-id="bd9ff-159">**NX_PPPOE_SERVER_THREAD_TIME_SLICE**: PPPoE sunucu iş parçacığı için zaman dilimi seçeneği.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-159">**NX_PPPOE_SERVER_THREAD_TIME_SLICE**: Time-slice option for PPPoE Server thread.</span></span> <span data-ttu-id="bd9ff-160">Varsayılan olarak, bu değer TX_NO_TIME_SLICE.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-160">By default, this value is TX_NO_TIME_SLICE.</span></span>

- <span data-ttu-id="bd9ff-161">**NX_PPPOE_SERVER_MAX_CLIENT_SESSION_NUMBER**: Bu, eşzamanlı istemci oturumlarının maksimum sayısını tanımlar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-161">**NX_PPPOE_SERVER_MAX_CLIENT_SESSION_NUMBER**: This defines the max number of concurrent client sessions.</span></span> <span data-ttu-id="bd9ff-162">Varsayılan olarak, bu değer 10 ' dur.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-162">By default, this value is 10.</span></span>

- <span data-ttu-id="bd9ff-163">**NX_PPPOE_SERVER_MAX_HOST_UNIQ_SIZE**: bu konak-Uniq 'ın maksimum boyutunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-163">**NX_PPPOE_SERVER_MAX_HOST_UNIQ_SIZE**: This defines the max size of Host-Uniq.</span></span> <span data-ttu-id="bd9ff-164">Varsayılan olarak, bu değer 32 ' dir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-164">By default, this value is 32.</span></span>

- <span data-ttu-id="bd9ff-165">**NX_PPPOE_SERVER_MAX_RELAY_SESSION_ID_SIZE**: Bu, maksimum geçiş-oturum kimliği boyutunu tanımlar. Varsayılan olarak, bu değer 12 ' dir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-165">**NX_PPPOE_SERVER_MAX_RELAY_SESSION_ID_SIZE**: This defines the max size of Relay-Session-Id. By default, this value is 12.</span></span>

- <span data-ttu-id="bd9ff-166">**NX_PPPOE_SERVER_MIN_PACKET_PAYLOAD_SIZE**: PPPoE sunucusu Için en düşük paket yükü boyutunu belirtir.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-166">**NX_PPPOE_SERVER_MIN_PACKET_PAYLOAD_SIZE**: Specifies the Minimum packet payload size for PPPoE Server.</span></span> <span data-ttu-id="bd9ff-167">Paket yükü boyutu bu değerden büyükse, paket zincirinden kaçınabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-167">If the packet payload size is greater than this value, can avoid packet chained.</span></span> <span data-ttu-id="bd9ff-168">Varsayılan olarak, bu değer 1520 (en fazla Ethernet 1500, Ethernet üstbilgisi 14, CRC 2 ve dört baytlık hizalama 4).</span><span class="sxs-lookup"><span data-stu-id="bd9ff-168">By default, this value is 1520 (Maximum Payload Size of Ethernet 1500, Ethernet Header 14, CRC 2 and Four-byte alignment 4).</span></span>

- <span data-ttu-id="bd9ff-169">**NX_PPPOE_SERVER_PACKET_TIMEOUT**: Bu, paket ayırmak veya paketlere veri eklemek için beklemeyi (Zamanlayıcı işaretleri) belirler.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-169">**NX_PPPOE_SERVER_PACKET_TIMEOUT**: This defines the wait potion(in timer ticks) for allocating packets or appending data into packets.</span></span> <span data-ttu-id="bd9ff-170">Varsayılan olarak, bu değer **NX_IP_PERIODIC_RATE** (100 Ticks).</span><span class="sxs-lookup"><span data-stu-id="bd9ff-170">By default, this value is **NX_IP_PERIODIC_RATE** (100 ticks).</span></span>

- <span data-ttu-id="bd9ff-171">**NX_PPPOE_SERVER_START_SESSION_ID**: Bu, PPPoE oturumuna atamaya yönelik başlangıç oturumu kimliğini tanımlar.</span><span class="sxs-lookup"><span data-stu-id="bd9ff-171">**NX_PPPOE_SERVER_START_SESSION_ID**: This defines the start Session ID for assigning to the PPPoE Session.</span></span> <span data-ttu-id="bd9ff-172">Varsayılan olarak, bu değer 0X4944 ' dir (KIMLIK için ASCII değeri).</span><span class="sxs-lookup"><span data-stu-id="bd9ff-172">By default, this value is 0X4944(ASCII value for ID).</span></span>