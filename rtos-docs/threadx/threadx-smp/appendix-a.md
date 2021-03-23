---
title: Ek A-Azure RTOS ThreadX SMP API hizmetleri
description: ThreadX SMP API hizmetleri
author: philmea
ms.author: philmea
ms.date: 06/04/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: a246bf997bfb51136c6a3802fe6b099d6a9002a4
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104827341"
---
# <a name="appendix-a---azure-rtos-threadx-smp-api-services"></a>Ek A-Azure RTOS ThreadX SMP API hizmetleri

## <a name="entry-function"></a>Entry Işlevi

```C
VOID     tx_kernel_enter(VOID);
```
## <a name="block-memory-services"></a>Bellek hizmetlerini engelle

```C
UINT     tx_block_allocate(TX_BLOCK_POOL *pool_ptr,
            VOID **block_ptr, ULONG wait_option);

UINT     tx_block_pool_create(TX_BLOCK_POOL *pool_ptr,
            CHAR *name_ptr, ULONG block_size,
            VOID *pool_start, ULONG pool_size);

UINT     tx_block_pool_delete(TX_BLOCK_POOL *pool_ptr);

UINT     tx_block_pool_info_get(TX_BLOCK_POOL
            *pool_ptr,
            CHAR **name,
            ULONG *available_blocks, ULONG
            *total_blocks,
            TX_THREAD **first_suspended,
            ULONG *suspended_count,
            TX_BLOCK_POOL **next_pool);

UINT
            tx_block_pool_performance_info_get(TX_BLOC
            K_POOL *pool_ptr,
            ULONG *allocates, ULONG *releases, ULONG
            *suspensions,
            ULONG *timeouts);

UINT
            tx_block_pool_performance_system_info_get(
            ULONG *allocates,
            ULONG *releases, ULONG *suspensions, ULONG
            *timeouts);

UINT         tx_block_pool_prioritize(TX_BLOCK_POOL
                *pool_ptr);

UINT         tx_block_release(VOID *block_ptr);
```
## <a name="byte-memory-services"></a>Bayt bellek Hizmetleri

```C
UINT     tx_byte_allocate(TX_BYTE_POOL *pool_ptr,
            VOID **memory_ptr,
            ULONG memory_size, ULONG wait_option);

UINT     tx_byte_pool_create(TX_BYTE_POOL *pool_ptr,
            CHAR *name_ptr,
            VOID *pool_start, ULONG pool_size);

UINT     tx_byte_pool_delete(TX_BYTE_POOL *pool_ptr);

UINT     tx_byte_pool_info_get(TX_BYTE_POOL *pool_ptr,
            CHAR **name, ULONG *available_bytes,
            ULONG *fragments, TX_THREAD
            **first_suspended,
            ULONG *suspended_count,
            TX_BYTE_POOL **next_pool);

UINT     tx_byte_pool_performance_info_get(TX_BYTE_POOL
            *pool_ptr,
            ULONG *allocates,
            ULONG *releases, ULONG *fragments_searched,
            ULONG *merges,
            ULONG *splits, ULONG *suspensions, ULONG
            *timeouts);

UINT     tx_byte_pool_performance_system_info_get(ULONG
            *allocates,
            ULONG *releases, ULONG *fragments_searched,
            ULONG *merges, ULONG *splits, ULONG
            *suspensions, ULONG *timeouts);

UINT     tx_byte_pool_prioritize(TX_BYTE_POOL
            *pool_ptr);

UINT     tx_byte_release(VOID *memory_ptr);
```
## <a name="event-flags-services"></a>Olay bayrakları Hizmetleri

```C
UINT     tx_event_flags_create(TX_EVENT_FLAGS_GROUP
            *group_ptr,
            CHAR *name_ptr);

UINT     tx_event_flags_delete(TX_EVENT_FLAGS_GROUP
            *group_ptr);

UINT     tx_event_flags_get(TX_EVENT_FLAGS_GROUP
            *group_ptr,
            ULONG requested_flags, UINT get_option,
            ULONG *actual_flags_ptr, ULONG
            wait_option);

UINT     tx_event_flags_info_get(TX_EVENT_FLAGS_GROUP
            *group_ptr,
            CHAR **name, ULONG *current_flags,
            TX_THREAD **first_suspended,
            ULONG *suspended_count,
            TX_EVENT_FLAGS_GROUP **next_group);

UINT
            tx_event_flags_performance_info_get(TX_EVE
            NT_FLAGS_GROUP *group_ptr, ULONG *sets,
            ULONG *gets, ULONG *suspensions,
            ULONG *timeouts);

UINT
            tx_event_flags_performance_system_info_get
            (ULONG *sets, ULONG *gets,
            ULONG *suspensions, ULONG *timeouts);

UINT     tx_event_flags_set(TX_EVENT_FLAGS_GROUP
            *group_ptr,
            ULONG flags_to_set, UINT set_option);

UINT     tx_event_flags_set_notify(TX_EVENT_FLAGS_GROUP
            *group_ptr,
            VOID
            (*events_set_notify)(TX_EVENT_FLAGS_GROUP
            *));
```
## <a name="interrupt-control"></a>Kesme denetimi

```C
UINT     tx_interrupt_control(UINT new_posture);
```
## <a name="mutex-services"></a>Mutex Hizmetleri

```C
UINT     tx_mutex_create(TX_MUTEX *mutex_ptr, CHAR
            *name_ptr,
            UINT inherit);

UINT     tx_mutex_delete(TX_MUTEX *mutex_ptr);

UINT     tx_mutex_get(TX_MUTEX *mutex_ptr, ULONG
            wait_option);

UINT     tx_mutex_info_get(TX_MUTEX *mutex_ptr, CHAR
            **name,
            ULONG *count, TX_THREAD **owner,
            TX_THREAD **first_suspended,
            ULONG *suspended_count,
            TX_MUTEX **next_mutex);

UINT     tx_mutex_performance_info_get(TX_MUTEX
            *mutex_ptr, ULONG *puts, ULONG *gets, ULONG
            *suspensions, ULONG *timeouts,
            ULONG *inversions, ULONG *inheritances);

UINT     tx_mutex_performance_system_info_get(ULONG
            *puts, ULONG *gets,
            ULONG *suspensions, ULONG *timeouts, ULONG
            *inversions,
            ULONG *inheritances);

UINT     tx_mutex_prioritize(TX_MUTEX *mutex_ptr);

UINT     tx_mutex_put(TX_MUTEX *mutex_ptr);
```
## <a name="queue-services"></a>Kuyruk Hizmetleri

```C
UINT     tx_queue_create(TX_QUEUE *queue_ptr, CHAR
            *name_ptr,
            UINT message_size, VOID *queue_start,
            ULONG queue_size);

UINT     tx_queue_delete(TX_QUEUE *queue_ptr);

UINT     tx_queue_flush(TX_QUEUE *queue_ptr);

UINT     tx_queue_front_send(TX_QUEUE *queue_ptr, VOID
            *source_ptr,
            ULONG wait_option);

UINT     tx_queue_info_get(TX_QUEUE *queue_ptr, CHAR
            **name,
            ULONG *enqueued, ULONG *available_storage,
            TX_THREAD **first_suspended,
            ULONG *suspended_count, TX_QUEUE
            **next_queue);

UINT     tx_queue_performance_info_get(TX_QUEUE
            *queue_ptr,
            ULONG *messages_sent, ULONG
            *messages_received,
            ULONG *empty_suspensions, ULONG
            *full_suspensions,
            ULONG *full_errors, ULONG *timeouts);

UINT     tx_queue_performance_system_info_get(ULONG
            *messages_sent,
            ULONG *messages_received, ULONG
            *empty_suspensions,
            ULONG *full_suspensions, ULONG
            *full_errors,
            ULONG *timeouts);

UINT     tx_queue_prioritize(TX_QUEUE *queue_ptr);

UINT     tx_queue_receive(TX_QUEUE *queue_ptr,
            VOID *destination_ptr, ULONG wait_option);

UINT     tx_queue_send(TX_QUEUE *queue_ptr, VOID
            *source_ptr,
            ULONG wait_option);

UINT     tx_queue_send_notify(TX_QUEUE *queue_ptr, VOID
            (*queue_send_notify)(TX_QUEUE *));
```
## <a name="semaphore-services"></a>Semafor Hizmetleri

```C
UINT     tx_semaphore_ceiling_put(TX_SEMAPHORE
            *semaphore_ptr,
            ULONG ceiling);

UINT     tx_semaphore_create(TX_SEMAPHORE
            *semaphore_ptr,
            CHAR *name_ptr, ULONG initial_count);

UINT     tx_semaphore_delete(TX_SEMAPHORE
            *semaphore_ptr);

UINT     tx_semaphore_get(TX_SEMAPHORE *semaphore_ptr,
            ULONG wait_option);

UINT     tx_semaphore_info_get(TX_SEMAPHORE
            *semaphore_ptr, CHAR **name,
            ULONG *current_value,
            TX_THREAD **first_suspended,
            ULONG *suspended_count,
            TX_SEMAPHORE **next_semaphore);

UINT     tx_semaphore_performance_info_get(TX_SEMAPHORE
            *semaphore_ptr,
            ULONG *puts, ULONG *gets, ULONG
            *suspensions,
            ULONG *timeouts);

UINT     tx_semaphore_performance_system_info_get(ULONG
            *puts,
            ULONG *gets, ULONG *suspensions, ULONG
            *timeouts);

UINT     tx_semaphore_prioritize(TX_SEMAPHORE
            *semaphore_ptr);

UINT     tx_semaphore_put(TX_SEMAPHORE *semaphore_ptr);

UINT     tx_semaphore_put_notify(TX_SEMAPHORE
            *semaphore_ptr,
            VOID (*semaphore_put_notify)(TX_SEMAPHORE
            *));
```
## <a name="thread-control-services"></a>İş parçacığı denetim hizmetleri

```C
UINT     tx_thread_create(TX_THREAD *thread_ptr,
            CHAR *name_ptr,
            VOID (*entry_function)(ULONG), ULONG
            entry_input,
            VOID *stack_start, ULONG stack_size,
            UINT priority, UINT preempt_threshold,
            ULONG time_slice, UINT auto_start);

UINT     tx_thread_delete(TX_THREAD *thread_ptr);

UINT     tx_thread_entry_exit_notify(TX_THREAD
            *thread_ptr,
            VOID (*thread_entry_exit_notify)(TX_THREAD
            *, UINT));

TX_THREAD *tx_thread_identify(VOID);

UINT     tx_thread_info_get(TX_THREAD *thread_ptr, CHAR
            **name,
            UINT *state, ULONG *run_count, UINT
            *priority,
            UINT *preemption_threshold, ULONG
            *time_slice,
            TX_THREAD **next_thread,
            TX_THREAD **next_suspended_thread);

UINT     tx_thread_performance_info_get(TX_THREAD
            *thread_ptr,
            ULONG *resumptions, ULONG *suspensions,
            ULONG *solicited_preemptions,
            ULONG *interrupt_preemptions,
            ULONG *priority_inversions,ULONG
            *time_slices, ULONG *relinquishes, ULONG
            *timeouts,
            ULONG *wait_aborts, TX_THREAD
            **last_preempted_by);

UINT     tx_thread_performance_system_info_get(ULONG
            *resumptions,
            ULONG *suspensions,
            ULONG *solicited_preemptions,
            ULONG *interrupt_preemptions,
            ULONG *priority_inversions,ULONG
            *time_slices, ULONG *relinquishes, ULONG
            *timeouts,
            ULONG *wait_aborts, ULONG
            *non_idle_returns,
            ULONG *idle_returns);

UINT     tx_thread_preemption_change(TX_THREAD
            *thread_ptr,
            UINT new_threshold, UINT *old_threshold);

UINT     tx_thread_priority_change(TX_THREAD
            *thread_ptr,
            UINT new_priority, UINT *old_priority);

VOID     tx_thread_relinquish(VOID);

UINT     tx_thread_reset(TX_THREAD *thread_ptr);

UINT     tx_thread_resume(TX_THREAD *thread_ptr);

UINT     tx_thread_sleep(ULONG timer_ticks);

UINT     tx_thread_smp_core_exclude(TX_THREAD
            *thread_ptr,
            ULONG exclusion_map);

UINT     tx_thread_smp_core_exclude_get(TX_THREAD
            *thread_ptr,
            ULONG *exclusion_map_ptr);

UINT     tx_thread_smp_core_get(void);

UINT     tx_thread_stack_error_notify
            VOID(*stack_error_handler)(TX_THREAD *));

UINT     tx_thread_suspend(TX_THREAD *thread_ptr);

UINT     tx_thread_terminate(TX_THREAD *thread_ptr);

UINT     tx_thread_time_slice_change(TX_THREAD
            *thread_ptr,
            ULONG new_time_slice, ULONG
            *old_time_slice);

UINT     tx_thread_wait_abort(TX_THREAD *thread_ptr);
```
## <a name="time-services"></a>Zaman hizmetleri

```C
ULONG     tx_time_get(VOID);
VOID      tx_time_set(ULONG new_time);
```
## <a name="timer-services"></a>Zamanlayıcı Hizmetleri

```C
UINT     tx_timer_activate(TX_TIMER *timer_ptr);

UINT     tx_timer_change(TX_TIMER *timer_ptr,
            ULONG initial_ticks,
            ULONG reschedule_ticks);

UINT     tx_timer_create(TX_TIMER *timer_ptr,
            CHAR *name_ptr,
            VOID (*expiration_function)(ULONG),
            ULONG expiration_input, ULONG
            initial_ticks,
            ULONG reschedule_ticks, UINT
            auto_activate);

UINT     tx_timer_deactivate(TX_TIMER *timer_ptr);

UINT     tx_timer_delete(TX_TIMER *timer_ptr);

UINT     tx_timer_info_get(TX_TIMER *timer_ptr, CHAR
            **name,
            UINT *active, ULONG *remaining_ticks,
            ULONG *reschedule_ticks,
            TX_TIMER **next_timer);

UINT     tx_timer_performance_info_get(TX_TIMER
            *timer_ptr, ULONG *activates,
            ULONG *reactivates, ULONG *deactivates,
            ULONG *expirations,
            ULONG *expiration_adjusts);

UINT     tx_timer_performance_system_info_get
            ULONG *activates, ULONG *reactivates,
            ULONG *deactivates, ULONG *expirations,
            ULONG *expiration_adjusts);

UINT     tx_timer_smp_core_exclude(TX_TIMER *timer_ptr,
            ULONG exclusion_map);

UINT     tx_timer_smp_core_exclude_get(TX_TIMER
            *timer_ptr,
            ULONG *exclusion_map_ptr);
```