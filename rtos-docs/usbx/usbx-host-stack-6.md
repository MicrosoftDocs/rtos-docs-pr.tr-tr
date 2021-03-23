---
title: Bölüm 6-USBX CDC-ECD sınıf kullanımı
description: USBX, konak ve cihaz tarafı için bir CDC-ECD sınıfı içerir. Bu sınıf, NetX ile kullanılmak üzere tasarlanmıştır, özellikle USBX CDC-ECD sınıfı NetX sürücüsü olarak davranır. Bu nedenle Bölüm 5 ' te hiçbir CDC-ECD API 'si yoktur.
author: philmea
ms.author: philmea
ms.date: 5/19/2020
ms.service: rtos
ms.topic: article
ms.openlocfilehash: 18e7e075788623916de36cf911597230295b56c5
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104828438"
---
# <a name="chapter-6---usbx-cdc-ecm-class-usage"></a>Bölüm 6-USBX CDC-ECD sınıf kullanımı

USBX, konak ve cihaz tarafı için bir CDC-ECD sınıfı içerir. Bu sınıf, NetX ile kullanılmak üzere tasarlanmıştır, özellikle USBX CDC-ECD sınıfı NetX sürücüsü olarak davranır. Bu nedenle Bölüm 5 ' te hiçbir CDC-ECD API 'si yoktur.

NetX ve USBX başlatıldıktan ve USBX tarafından bir CDC-ECı cihazının bir örneği bulunursa, uygulama, cihaz ile iletişim kurmak için özel olarak NetX kullanır. Başlatma aşağıdaki örnekte gösterilen kalıbı izler.

```c
UINT status;

/* The USB controller should be the last component initialized so that
everything is ready when data starts being received. */

/* Initialize USBX. */

ux_system_initialize(memory_pointer, UX_USBX_MEMORY_SIZE, UX_NULL, 0);

/* The code below is required for installing the host portion of USBX */
status = ux_host_stack_initialize(UX_NULL);

/* Register cdc_ecm class. */

status = ux_host_stack_class_register(_ux_system_host_class_cdc_ecm_name,
    ux_host_class_cdc_ecm_entry);

/* Perform the initialization of the network driver. */

_ux_network_driver_init();

/* Initialize NetX. Refer to NetX user guide for details to add initialization code. */

/* Register the platform-specific USB controller. */

status = ux_host_stack_hcd_register("controller_name", controller_entry, param1, param2);

/* Find the CDC-ECM class. */
class_cdc_ecm_get();

/* Now wait for the link to be up. */

while (cdc_ecm -> ux_host_class_cdc_ecm_link_state != UX_HOST_CLASS_CDC_ECM_LINK_STATE_UP)
    tx_thread_sleep(10);

/* At this point, everything has been initialized, and we've found a CDC-ECM device.
    Now NetX can be used to communicate with the device. */
```
