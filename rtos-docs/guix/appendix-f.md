---
title: Ek F-Gux RTOS bağlama hizmetleri
description: GUX RTOS bağlama hizmetleri hakkında bilgi edinin.
author: philmea
ms.author: philmea
ms.date: 05/19/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 1d94dbb9d7d53ec3e1900188142974cc981dfea9
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104827269"
---
# <a name="appendix-f---guix-rtos-binding-services"></a><span data-ttu-id="e18d1-103">Ek F-Gux RTOS bağlama hizmetleri</span><span class="sxs-lookup"><span data-stu-id="e18d1-103">Appendix F - GUIX RTOS Binding Services</span></span>

<span data-ttu-id="e18d1-104">GUX, temel alınan RTOS tarafından sağlanan iş parçacığı veya görev Hizmetleri, mutex, olay kuyruğu ve zamanlama Hizmetleri gerektirir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-104">GUIX requires thread or tasking services, mutex, event queue, and timing services providing by the underlying RTOS.</span></span> <span data-ttu-id="e18d1-105">Varsayılan olarak Gux, bu hizmetleri sağlamak için ThreadX gerçek zamanlı işletim sistemini kullanacak şekilde yapılandırılmıştır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-105">By default GUIX is configured to utilize the ThreadX real time operating system to provide these services.</span></span> <span data-ttu-id="e18d1-106">Farklı bir işletim sistemine Gux bağlantı noktası için, geliştirici, ThreadX bağımlılıklarını kaldırmak için GX_DISABLE_THREADX_BINDING ön işlemci yönergesini tanımlamalıdır ve Gux kitaplığını yeniden derlemelidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-106">To port GUIX to another operating system, the developer should # define the pre-processor directive GX_DISABLE_THREADX_BINDING and rebuild the GUIX library to remove the ThreadX dependencies.</span></span> <span data-ttu-id="e18d1-107">Ayrıca, geliştiricinin aşağıdaki makro tanımlarını ve destekleyici işlevleri sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-107">In addition, the developer will need to provide the following macro definitions and supporting functions.</span></span> <span data-ttu-id="e18d1-108">Bu makro tanımlarının örnekleri ve destekleyici işlevler, örnek bir genel RTO 'lar tümleştirmesi sağlayan gx_system_rtos_bind. h ve gx_system_rtos_bind. c dosyalarında bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-108">Examples of these macro definitions and supporting functions can be found in the files gx_system_rtos_bind.h and gx_system_rtos_bind.c, which provide an example generic rtos integration.</span></span>

<span data-ttu-id="e18d1-109">Sistem tümleştirme makroları:</span><span class="sxs-lookup"><span data-stu-id="e18d1-109">System Integration macros:</span></span>

<span data-ttu-id="e18d1-110">**GX_RTOS_BINDING_INITIALIZE**</span><span class="sxs-lookup"><span data-stu-id="e18d1-110">**GX_RTOS_BINDING_INITIALIZE**</span></span>

<span data-ttu-id="e18d1-111">Bu makro sistem başlatma sırasında çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-111">This macro is invoked during system initialization.</span></span> <span data-ttu-id="e18d1-112">Bu makro, kullanılmadan önce RTO 'lar sistem hizmetlerinizi veya RTO 'lar kaynaklarınızı hazırlamak için gereken herhangi bir işlevi çağırmak üzere tanımlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-112">The macro should be defined to call any function needed to prepare your rtos system services or rtos resources prior to use.</span></span> <span data-ttu-id="e18d1-113">Bu, Gux 'in kullanacağı RTO 'lar kaynaklarını hazırlamak için bağlamanın fırsatına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-113">This is the binding’s opportunity to prepare the rtos resources that GUIX will use.</span></span>

<span data-ttu-id="e18d1-114">**GX_SYSTEM_THREAD_START**</span><span class="sxs-lookup"><span data-stu-id="e18d1-114">**GX_SYSTEM_THREAD_START**</span></span>

<span data-ttu-id="e18d1-115">Bu makro, Gux görevi veya iş parçacığının yürütülmeye başlaması gerektiğinde çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-115">This macro is invoked when the GUIX task or thread should start executing.</span></span> <span data-ttu-id="e18d1-116">Bu makro, çalışan Gux iş parçacığını başlatacak bir işlevi çağırmak için tanımlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-116">This macro should be defined to call a function which will start the GUIX thread running.</span></span> <span data-ttu-id="e18d1-117">GUX iş parçacığına giriş noktası çağrılan işleve geçirilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-117">The entry point to the GUIX thread is passed to the called function.</span></span> <span data-ttu-id="e18d1-118">Çağrılan işlevin imzası olmalıdır</span><span class="sxs-lookup"><span data-stu-id="e18d1-118">The signature of the called function must be</span></span>

<span data-ttu-id="e18d1-119">**UINT *function_name*(void (thread_entry_point) (void));**</span><span class="sxs-lookup"><span data-stu-id="e18d1-119">**UINT *function_name*(VOID (thread_entry_point)(VOID));**</span></span>

<span data-ttu-id="e18d1-120">Bu işlev, iş parçacığı başarıyla başlatılmışsa veya GX_FAILURE GX_SUCCESS döndürmelidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-120">This function should return GX_SUCCESS if the thread is successfully started, or GX_FAILURE.</span></span>

<span data-ttu-id="e18d1-121">**GX_EVENT_PUSH**</span><span class="sxs-lookup"><span data-stu-id="e18d1-121">**GX_EVENT_PUSH**</span></span>

<span data-ttu-id="e18d1-122">Bu makro, bir olayı Gux tarafından kullanılan FıFO olay kuyruğuna göndermek için çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-122">This macro is invoked to push an event into the FIFO event queue used by GUIX.</span></span> <span data-ttu-id="e18d1-123">Yeni bir RTOS 'a taşıma yaparken, bu olay kuyruğunu iş parçacığı güvenli bir şekilde uygulamak sizin sorumluluğunuzdadır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-123">When porting to a new rtos, it is your responsibility to implement this event queue in a thread-safe manner.</span></span> <span data-ttu-id="e18d1-124">GX_EVENT yapılar bu kuyruğa kopyalanmalıdır ve bu kuyruktan kopyalanmalıdır, yani Gux olayları olay üreticisi görünümünden otomatik değişkenler olduğundan, GX_EVENT işaretçilerin bir sırası çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="e18d1-124">GX_EVENT structures must be copied into this queue and copied out of this queue, i.e. a queue of GX_EVENT pointers will not work, since GUIX events can be automatic variables from the view of the event producer.</span></span> <span data-ttu-id="e18d1-125">Bu makro tarafından çağrılan işlevin imzası şu olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="e18d1-125">The signature of the function called by this macro must be:</span></span>

<span data-ttu-id="e18d1-126">\**UINT *function_name* (GX_EVENT *event_ptr);**</span><span class="sxs-lookup"><span data-stu-id="e18d1-126">\**UINT *function_name* (GX_EVENT *event_ptr);**</span></span>

<span data-ttu-id="e18d1-127">Olay olay kuyruğuna itilse, bu işlev GX_SUCCESS döndürmelidir, aksi takdirde GX_FAILURE döndürmelidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-127">This function should return GX_SUCCESS if the event is pushed into the event queue, otherwise it should return GX_FAILURE.</span></span>

<span data-ttu-id="e18d1-128">**GX_EVENT_POP**</span><span class="sxs-lookup"><span data-stu-id="e18d1-128">**GX_EVENT_POP**</span></span>

<span data-ttu-id="e18d1-129">Bu makro, GUIX olay kuyruğundan baş (en eski) olayı kaldırmak ve istenen konuma kopyalamak için çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-129">This macro is invoked to remove the head (oldest) event from the GUIX event queue and copy it into the requested location.</span></span> <span data-ttu-id="e18d1-130">Bu işlev, şu anda olay kuyruğunda hiçbir olay yoksa bir olayı bloke edebilir veya bekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-130">This function must be able to optionally block or wait for an event if no events are currently in the event queue.</span></span> <span data-ttu-id="e18d1-131">Bu makro tarafından çağrılan işlevin imzası olmalıdır</span><span class="sxs-lookup"><span data-stu-id="e18d1-131">The signature of the function invoked by this macro must be</span></span>

<span data-ttu-id="e18d1-132">UINT function_name (GX_EVENT \* put_event, GX_BOOL bekle)</span><span class="sxs-lookup"><span data-stu-id="e18d1-132">UINT function_name(GX_EVENT \*put_event, GX_BOOL wait)</span></span>

<span data-ttu-id="e18d1-133">Wait parametresi = = GX_TRUE, işlev bir olay sağlanana kadar döndürülmemelidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-133">If the wait parameter == GX_TRUE, the function should not return until an event is provided.</span></span> <span data-ttu-id="e18d1-134">Wait parametresi GX_FALSE ise, işlev hemen veya bir olay olmadan hemen döndürmelidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-134">If the wait parameter is GX_FALSE, the function should return immediately with or without an event.</span></span>

<span data-ttu-id="e18d1-135">Kuyruktan bir olay alınırsa, put_event konumuna kopyalanması ve dönüş durumunun GX_SUCCESS olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-135">If an event is retrieved from the queue, it should copied into the put_event location and the return status is GX_SUCCESS.</span></span> <span data-ttu-id="e18d1-136">Aksi takdirde, dönüş durumu GX_FAILURE olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-136">Otherwise the return status should be GX_FAILURE.</span></span>

<span data-ttu-id="e18d1-137">**GX_EVENT_FOLD**</span><span class="sxs-lookup"><span data-stu-id="e18d1-137">**GX_EVENT_FOLD**</span></span>

<span data-ttu-id="e18d1-138">Bu makro, bir olayı FıFO olay kuyruğuna katlamak için GUıDX tarafından çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-138">This macro is invoked by GUIX to fold an event into the FIFO event queue.</span></span> <span data-ttu-id="e18d1-139">Bir olayın katlaması, aynı türde bir olay kuyrukta zaten mevcutsa, bu girişin yeni olayın yükünü içerecek şekilde güncelleştirilmesi anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-139">Folding an event means that if an event of the same type already exists in the queue, that entry is update to contain the payload of the new event.</span></span> <span data-ttu-id="e18d1-140">Kuyrukta aynı türden mevcut bir olay bulunamazsa, sıraya yeni bir olay gönderilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-140">If an existing event of the same type is not found in the queue, a new event is pushed into the queue.</span></span> 

<span data-ttu-id="e18d1-141">Olay katlama özelliğini uygulayamayacağı bağlamalar için, GX_EVENT_PUSH çağırmak kabul edilebilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-141">For bindings that cannot implement the event fold feature, it is acceptable to simply invoke the GX_EVENT_PUSH.</span></span>

<span data-ttu-id="e18d1-142">**GX_TIMER_START**</span><span class="sxs-lookup"><span data-stu-id="e18d1-142">**GX_TIMER_START**</span></span>

<span data-ttu-id="e18d1-143">Bu makro, GUıDX ' in dönemsel süreölçer girişi alması gerektiğinde çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-143">This macro is invoked when GUIX needs to receive periodic timer input.</span></span> <span data-ttu-id="e18d1-144">Bu makro alt düzey RTOS dönemsel Zamanlayıcı hizmetini başlatan bir hizmeti çağırmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-144">This macro should invoke a service that starts the low-level RTOS periodic timer service.</span></span> <span data-ttu-id="e18d1-145">RTOS Zamanlayıcı hizmeti kolayca durdurulup başlayamadığında, bu hizmeti her zaman çalışır durumda bırakmak kabul edilebilir ancak daha az verimlidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-145">If the RTOS timer service cannot be easily stopped and started, it is acceptable but less efficient to leave this service running at all times.</span></span>

<span data-ttu-id="e18d1-146">Düşük düzey RTOS Zamanlayıcı hizmetinin süresi dolduğunda, bağlama Gux sistem işlevini çağırmalıdır _gx_system_timer_expiration (0); Bu işlevi düzenli aralıklarla çağırmak, üst düzey Gux Zamanlayıcı pencere öğesi Zamanlayıcı hizmetlerinin hangi sürücülerindedir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-146">When the low-level RTOS timer service periodically expires, the binding must call the GUIX system function _gx_system_timer_expiration(0); Calling this function periodically is what drives the high-level GUIX timer widget timer services.</span></span>

<span data-ttu-id="e18d1-147">**GX_TIMER_STOP**</span><span class="sxs-lookup"><span data-stu-id="e18d1-147">**GX_TIMER_STOP**</span></span>

<span data-ttu-id="e18d1-148">Bu makro, GUIX 'in artık düzenli bir zamanlayıcıya ihtiyaç duymuyorsa çağrılır (yani, etkin bir Gux zamanlayıcının çalışması yoktur).</span><span class="sxs-lookup"><span data-stu-id="e18d1-148">This macro is invoked when GUIX no longer needs a periodic timer (i.e. there are no active GUIX timers running).</span></span> <span data-ttu-id="e18d1-149">RTOS Zamanlayıcı hizmeti kolayca durdurulup başlayamıyorsa, bu hizmeti her zaman çalışır durumda bırakmak ve hiçbir şey yapmak için bu makroyu tanımlamak kabul edilebilir ancak daha az verimlidir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-149">If the RTOS timer service cannot be easily stopped and started, it is acceptable but less efficient to leave this service running at all times and define this macro to do nothing.</span></span>

<span data-ttu-id="e18d1-150">**GX_SYSTEM_MUTEX_LOCK**</span><span class="sxs-lookup"><span data-stu-id="e18d1-150">**GX_SYSTEM_MUTEX_LOCK**</span></span>

<span data-ttu-id="e18d1-151">Bu makro, kritik kod bölümleri sırasında, diğer bir görevin ortak veri yapılarını önceden oluşmasını ve değiştirmesini engellemek için, büyük olasılıkla bozulmaya neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-151">This macro is invoked by GUIX during critical code sections to prevent another task from  pre-empting and modifying common data structures, potentially causing corruption.</span></span> <span data-ttu-id="e18d1-152">Bu makro uygun RTOS kaynak kilitleme hizmetini uygulayan bir işlev çağırmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-152">This macro should call a function that implements the suitable RTOS resource locking service.</span></span>

<span data-ttu-id="e18d1-153">GUX iş parçacığı dışında hiçbir şekilde Gux API hizmeti kullanmıyorsanız, hiçbir şey yapmak için bu makroyu tanımlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e18d1-153">If you never utilize any GUIX API services outside of the GUIX thread, you can define this macro to do nothing.</span></span>

<span data-ttu-id="e18d1-154">**GX_SYSTEM_MUTEX_UNLOCK**</span><span class="sxs-lookup"><span data-stu-id="e18d1-154">**GX_SYSTEM_MUTEX_UNLOCK**</span></span>

<span data-ttu-id="e18d1-155">Bu makro, kritik kod bölümlerinin sonunda çağrılır ve uygun temel alınan RTOS hizmetini kullanarak Gux kaynağının kilidini açmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-155">This macro is invoked at the end of critical code sections, and should unlock the GUIX resource using the suitable underlying RTOS service.</span></span> <span data-ttu-id="e18d1-156">GUX iş parçacığı dışında hiçbir şekilde Gux API hizmeti kullanmıyorsanız, hiçbir şey yapmak için bu makroyu tanımlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e18d1-156">If you never utilize any GUIX API services outside of the GUIX thread, you can define this macro to do nothing.</span></span>

<span data-ttu-id="e18d1-157">**GX_SYSTEM_TIME_GET**</span><span class="sxs-lookup"><span data-stu-id="e18d1-157">**GX_SYSTEM_TIME_GET**</span></span>

<span data-ttu-id="e18d1-158">Bu makro, genellikle sistem başlangıcından bu yana gerçekleşen alt düzey Zamanlayıcı kesmelerinin sayısı olan "sistem işaretleri" olan geçerli sistem saatini döndüren bir işlevi çağırmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-158">This macro should call a function that returns the current system time is “system ticks”, which is usually the number of low-level timer interrupts that have occurred since system startup.</span></span> <span data-ttu-id="e18d1-159">Bu hizmet, dokunma girişi hareketleri için dokunma olayı kalem hızını hesaplamak için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-159">This service is used to calculate touch event pen speed for touch input gestures.</span></span> <span data-ttu-id="e18d1-160">Bu makro tarafından çağrılan işlevin imzası şu olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="e18d1-160">The signature of the function invoked by this macro must be:</span></span>

<span data-ttu-id="e18d1-161">**ULONG *function_name*(VOID);**</span><span class="sxs-lookup"><span data-stu-id="e18d1-161">**ULONG *function_name*(VOID);**</span></span>

<span data-ttu-id="e18d1-162">**GX_CURRENT_THREAD**</span><span class="sxs-lookup"><span data-stu-id="e18d1-162">**GX_CURRENT_THREAD**</span></span>

<span data-ttu-id="e18d1-163">Bu makro, yürütülmekte olan iş parçacığını belirlemek için çağrılır.</span><span class="sxs-lookup"><span data-stu-id="e18d1-163">This macro is invoked to identify the currently executing thread.</span></span> <span data-ttu-id="e18d1-164">Bu makro tarafından çağrılan hizmetin bir void \* döndürmesi gerekir, yani işletim sisteminiz tarafından geçerli yürütme iş parçacığını tanımlamak için kullanılan veri türünün GUX olarak döndürülmek üzere void \* olarak dönüştürülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="e18d1-164">The service called by this macro must return a void \*, meaning that the data type used by your operating system to identify the current execution thread must be cast to a void \* to be returned to GUX.</span></span>

<span data-ttu-id="e18d1-165">Bir genel RTOS bağlamasının tamamı bir örneği, dosyalanmış gx_system_rtos_bind. h ve gx_system_rtos_bind. c ' de uygulanır</span><span class="sxs-lookup"><span data-stu-id="e18d1-165">A complete example of a generic RTOS binding is implemented in the filed gx_system_rtos_bind.h and gx_system_rtos_bind.c</span></span>