---
title: Получение общего или делегированного календаря Outlook и его событий
description: В Outlook владелец календаря может поделиться им с другими пользователями и предоставить им доступ на просмотр или изменение событий в своем календаре. Календарь может быть пользовательским или основным. Владелец также может предоставить делегату право выполнять действия от его имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в основном календаре учетной записи электронной почты.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 06e11f11b9c25e3392075e027278558d1330d51e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470076"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a><span data-ttu-id="2fbdc-104">Получение общего или делегированного календаря Outlook и его событий</span><span class="sxs-lookup"><span data-stu-id="2fbdc-104">Get shared or delegated Outlook calendar and its events</span></span>

<span data-ttu-id="2fbdc-105">В Outlook владелец календаря может поделиться им с другими пользователями и предоставить им доступ на просмотр или изменение событий в своем календаре. Общий календарь может быть основным календарем владельца или пользовательским календарем, созданным владельцем.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-105">In Outlook, a calendar owner can share a calendar with other users and let them view or modify events in that calendar; the shared calendar can be the owner's primary calendar or a custom calendar created by the owner.</span></span> <span data-ttu-id="2fbdc-106">Владелец также может предоставить делегату для своего основного календаря право выполнять действия от его имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в основном календаре.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-106">The owner can also grant a delegate to their primary calendar and act on their behalf, to receive or respond to meeting requests, or create or change items in the primary calendar.</span></span>

<span data-ttu-id="2fbdc-107">Что касается программного кода, Microsoft Graph поддерживает чтение и запись событий в календарях, доступ к которым был предоставлен другими пользователями, а также чтение общих календарей и обновление их имен для получателей общего доступа.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-107">Programmatically, Microsoft Graph supports reading and writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="2fbdc-108">Поддержка также относится к делегированным календарям.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="2fbdc-109">Далее в этой статье описывается чтение событий в общем или делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-109">The rest of this article describes reading events in a shared or delegated calendar.</span></span> <span data-ttu-id="2fbdc-110">Сведения о создании событий см. в статье [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2fbdc-110">For creating events, refer to [Create Outlook events in a shared or delegated calendar](outlook-create-event-in-shared-delegated-calendar.md).</span></span>

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a><span data-ttu-id="2fbdc-111">Получатель общего доступа: получение общего календаря или его событий непосредственно из почтового ящика владельца календаря</span><span class="sxs-lookup"><span data-stu-id="2fbdc-111">Sharee: Get a shared calendar or its events directly from calendar owner's mailbox</span></span>

<span data-ttu-id="2fbdc-112">В трех примерах, приведенных ниже, используется следующий сценарий: Артем поделился своим основным календарем с Мартой в Outlook и предоставил ей разрешения на чтение.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-112">The three examples below use this scenario: in Outlook, Alex has shared his primary calendar with Megan and given Megan read permissions.</span></span> <span data-ttu-id="2fbdc-113">Если Марта войдет в приложение и предоставит _делегированные разрешения_ (Calendars.Read.Shared или Calendars.ReadWrite.Shared) от своего имени, приложение сможет получить доступ к основному календарю Артема и его событиям непосредственно из почтового ящика Артема.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-113">If Megan signs into your app and provides _delegated permissions_ (Calendars.Read.Shared or Calendars.ReadWrite.Shared), on behalf of Megan, your app can access Alex' primary calendar and its events directly from Alex' mailbox.</span></span>

<span data-ttu-id="2fbdc-114">В трех примерах указан идентификатор владельца (ИД пользователя или имя участника-пользователя Артема) и ярлык `calendar`.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-114">The three examples specify the owner's identity (Alex' user ID or user principal name) and the `calendar` shortcut.</span></span> <span data-ttu-id="2fbdc-115">У них есть доступ к идентификаторам календаря и событий, которые соответствуют почтовому ящику владельца.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-115">They access calendar and event IDs that correspond to only the owner's mailbox.</span></span> <span data-ttu-id="2fbdc-116">При указании идентификаторов календаря и событий в почтовом ящике получателя общего доступа (идентификатор пользователя или имя участника-пользователя Марты) будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-116">Specifying these calendar and event IDs in the sharee's mailbox (Megan's user ID or user principal name) would return an error.</span></span> <span data-ttu-id="2fbdc-117">Сведения об использовании идентификаторов календаря и событий, которые соответствуют почтовому ящику получателя общего доступа, см. в разделе [Получатель общего доступа: получение общего пользовательского календаря или его событий из почтового ящика получателя общего доступа](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span><span class="sxs-lookup"><span data-stu-id="2fbdc-117">To use calendar and event IDs that correspond to the sharee's mailbox, see [Sharee: Get shared, custom calendar or its events from sharee's mailbox](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span> 

> <span data-ttu-id="2fbdc-118">**Примечание.** Разрешения общего доступа (Calendars.Read.Shared или Calendars.ReadWrite.Shared) позволяют читать или записывать события в общем или делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-118">**Note**: The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="2fbdc-119">Они не поддерживают [подписку на уведомления об изменениях](webhooks.md) элементов в таких папках.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-119">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="2fbdc-120">Чтобы настроить подписки на уведомления об изменениях событий в общем, делегированном или любом другом календаре пользователя или ресурса в клиенте, используйте разрешение приложения Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-120">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="2fbdc-121">Марта: получение общего основного календаря непосредственно из почтового ящика Артема</span><span class="sxs-lookup"><span data-stu-id="2fbdc-121">Megan: Get the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="2fbdc-122">Войдя в систему под именем Марты, получите основной календарь, которым Артем поделился с Мартой, непосредственно из почтового ящика Артема.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-122">Signed in as Megan, get the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

<span data-ttu-id="2fbdc-123">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [calendar](/graph/api/resources/calendar?view=graph-rest-1.0), представляющий общий основной календарь Артема, в его почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-123">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Alex' shared, primary calendar, in Alex' mailbox.</span></span>

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="2fbdc-124">Марта: получение события общего основного календаря непосредственно из почтового ящика Артема</span><span class="sxs-lookup"><span data-stu-id="2fbdc-124">Megan: Get an event in the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="2fbdc-125">При выполнении входа в систему под именем Марты приложение может получить определенное событие основного календаря, которым Артем поделился с Мартой, непосредственно из его почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-125">Signed in as Megan, your app can get a specific event in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="2fbdc-126">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [event](/graph/api/resources/event?view=graph-rest-1.0), определенный параметром `{id}` в основном календаре Артема, непосредственно из его почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-126">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` in Alex' primary calendar, directly from Alex' mailbox.</span></span>

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a><span data-ttu-id="2fbdc-127">Марта: получение всех событий общего основного календаря из почтового ящика Артема</span><span class="sxs-lookup"><span data-stu-id="2fbdc-127">Megan: Get all the events in the shared, primary calendar from Alex' mailbox</span></span>

<span data-ttu-id="2fbdc-128">Войдя в систему под именем Марты, получите все события основного календаря, которым Артем поделился с Мартой, непосредственно из его почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-128">Signed in as Megan, get all the events in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

<span data-ttu-id="2fbdc-129">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [event](/graph/api/resources/event?view=graph-rest-1.0) в основном календаре Артема непосредственно из его почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-129">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Alex' primary calendar, directly from Alex' mailbox.</span></span>

<span data-ttu-id="2fbdc-130">Те же возможности GET доступны в том случае, если Артем делегировал Марте доступ к своему основному календарю или если Артем делегировал Марте весь свой почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-130">The same GET capabilities apply if Alex has delegated Megan access to Alex' primary calendar, or if Alex has delegated Megan his entire mailbox.</span></span>

<span data-ttu-id="2fbdc-131">Если Артем не предоставил общий доступ к своему основному календарю и не делегировал его Марте, при указании ИД пользователя или имени участника-пользователя Артема будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-131">If Alex has not shared nor delegated his primary calendar with Megan, specifying Alex’s user ID or user principal name in the preceding GET operations will return an error.</span></span> 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a><span data-ttu-id="2fbdc-132">Получатель общего доступа: получение общего пользовательского календаря или его событий из почтового ящика получателя общего доступа</span><span class="sxs-lookup"><span data-stu-id="2fbdc-132">Sharee: Get shared, custom calendar or its events from sharee's mailbox</span></span>

<span data-ttu-id="2fbdc-133">Если Артем поделился _пользовательским_ календарем (например, календарем «Детские праздники») с Анной и Анна предоставила делегированные разрешения (Calendars.Read или Calendars.ReadWrite), приложение может получить события или календарь из локальной копии календаря Артема в почтовом ящике Анны, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-133">If Alex has shared a _custom_ calendar (as an example, a calendar named "Kids parties") with Adele, and Adele has provided delegated permissions (Calendars.Read or Calendars.ReadWrite), your app can get the events or calendar from the local copy of Alex' calendar in Adele's mailbox, as described below.</span></span>

1. <span data-ttu-id="2fbdc-134">Войдя в систему под именем Анны, используйте один из следующих запросов, чтобы получить все календари, к которым Анна имеет доступ, в том числе общий пользовательский календарь.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-134">Signed in as Adele, use either of the following requests to get all the calendars that Adele has access to, including the shared custom calendar.</span></span>

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    <span data-ttu-id="2fbdc-135">Успешный отклик включает код ответа HTTP 200 и коллекцию календарей, к которым Анна имеет доступ, в том числе календарь («Детские праздники») с именем владельца, указанным как "Артем Кузнецов", в качестве второго календаря.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-135">A successful response includes the response code HTTP 200, and the collection of calendars that Adele has access to, including the calendar ("Kids parties") that has the owner name as "Alex Wilber" as the second calendar in the response.</span></span> <span data-ttu-id="2fbdc-136">Для получателя общего доступа, Анны, свойство **canShare** общего календаря всегда имеет значение "false".</span><span class="sxs-lookup"><span data-stu-id="2fbdc-136">For a sharee, Adele, the **canShare** property of the shared calendar is always false.</span></span>

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
      "truncated": true,
      "@odata.type": "microsoft.graph.calendar",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json

    {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
        "value": [
            {
                "id": "AQMkADU5NAAAJMjAAAAA==",
                "name": "Calendar",
                "color": "auto",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
                "canShare": true,
                "canViewPrivateItems": true,
                "canEdit": true,
                "owner": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            {
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. <span data-ttu-id="2fbdc-137">Войдя в систему под именем Анны, получите общий календарь или одно или несколько событий общего календаря, используя в отклике идентификатор второго календаря с шага 1.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-137">Signed in as Adele, get the shared calendar, or get one or more events in the shared calendar, using the second calendar ID in the response from step 1.</span></span> <span data-ttu-id="2fbdc-138">Идентификаторы общего календаря и его события соответствуют локальной копии календаря Артема в почтовом ящике Анны.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-138">The IDs of the shared calendar and its event correspond to the local copy of Alex' calendar in Adele's mailbox.</span></span>

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

<span data-ttu-id="2fbdc-139">В случае успешного выполнения вы получите отклик HTTP 200 ОК и запрошенное событие, события или календарь, которым Артем поделился с Анной.</span><span class="sxs-lookup"><span data-stu-id="2fbdc-139">On successful completion, you'll get HTTP 200 OK and the requested event, events, or calendar that Alex has shared with Adele.</span></span>


## <a name="next-steps"></a><span data-ttu-id="2fbdc-140">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2fbdc-140">Next steps</span></span>

<span data-ttu-id="2fbdc-141">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="2fbdc-141">Find out more about:</span></span>

- [<span data-ttu-id="2fbdc-142">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="2fbdc-142">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="2fbdc-143">Предоставление общего доступа к календарю или его делегирование в Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2fbdc-143">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="2fbdc-144">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="2fbdc-144">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="2fbdc-145">[API календаря](/graph/api/resources/calendar?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="2fbdc-145">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
