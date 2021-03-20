---
title: Создание событий Outlook в общем или делегированном календаре
description: В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e09b3552ca0d4a3ecd85855c471ec1cc16950abf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941402"
---
# <a name="create-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="3dc61-104">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="3dc61-104">Create Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="3dc61-105">В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать, создавать или изменять события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="3dc61-105">In Outlook, customers can share a calendar with other users and let them view, create, or modify events in that calendar.</span></span> <span data-ttu-id="3dc61-106">Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.</span><span class="sxs-lookup"><span data-stu-id="3dc61-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="3dc61-107">Что касается программного кода, Microsoft Graph поддерживает чтение и запись событий в календарях, доступ к которым был предоставлен другими пользователями, а также чтение общих календарей и обновление их имен для получателей общего доступа.</span><span class="sxs-lookup"><span data-stu-id="3dc61-107">Programmatically, Microsoft Graph supports reading or writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="3dc61-108">Поддержка также относится к делегированным календарям.</span><span class="sxs-lookup"><span data-stu-id="3dc61-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="3dc61-109">Далее в этой статье рассматривается создание собрания как нового события в общем или делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="3dc61-109">The rest of this article walks through creating a meeting event in a shared or delegated calendar.</span></span> <span data-ttu-id="3dc61-110">Сведения о получении событий см. в статье [Получение событий Outlook из общего или делегированного календаря](outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="3dc61-110">For getting events, refer to [Get Outlook events in a shared or delegated calendar](outlook-get-shared-events-calendars.md).</span></span>

<span data-ttu-id="3dc61-111">Приведенное ниже руководство содержит пример сценария, в котором Артем делегировал свой основной календарь Анне в Outlook и сохранил параметр почтового ящика Outlook по умолчанию, позволяющий направлять приглашения на собрание и ответы только делегатам.</span><span class="sxs-lookup"><span data-stu-id="3dc61-111">The walkthrough below uses the example scenario where Alex has delegated his primary calendar to Adele in Outlook, and kept the default Outlook mailbox setting to direct meeting requests and responses to only delegates.</span></span> <span data-ttu-id="3dc61-112">(Этот параметр соответствует свойству **delegateMeetingMessageDeliveryOptions** в [mailboxSettings](/graph/api/resources/mailboxsettings)Алекса, установленному в качестве значения по умолчанию `sendToDelegateOnly`.)</span><span class="sxs-lookup"><span data-stu-id="3dc61-112">(This setting corresponds to the **delegateMeetingMessageDeliveryOptions** property of Alex' [mailboxSettings](/graph/api/resources/mailboxsettings) set as the default value `sendToDelegateOnly`.)</span></span> 

<span data-ttu-id="3dc61-113">В этом руководстве описано несколько последующих шагов.</span><span class="sxs-lookup"><span data-stu-id="3dc61-113">The walkthrough describes a few subsequent steps:</span></span>
1. <span data-ttu-id="3dc61-114">[Анна получает календарь, делегированный Артемом](#step-1-adele-gets-the-delegated-calendar).</span><span class="sxs-lookup"><span data-stu-id="3dc61-114">[Adele gets the calendar that Alex has delegated to her](#step-1-adele-gets-the-delegated-calendar).</span></span>
2. <span data-ttu-id="3dc61-115">[Анна отправляет приглашение на собрание Алене и Марте от имени Артема](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf).</span><span class="sxs-lookup"><span data-stu-id="3dc61-115">[Adele sends a meeting invitation to Christie and Megan on Alex' behalf](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf).</span></span> 
3. <span data-ttu-id="3dc61-116">[Алена получает приглашение на собрание и изучает соответствующее событие в своем календаре](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).</span><span class="sxs-lookup"><span data-stu-id="3dc61-116">[Christie receives the meeting request, and inspects the associated event in her calendar](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).</span></span>
4. <span data-ttu-id="3dc61-117">[Алена помечает приглашение "Под вопросом"](#step-4-christie-responds-to-the-meeting-request).</span><span class="sxs-lookup"><span data-stu-id="3dc61-117">[Christie responds tentative to the invitation](#step-4-christie-responds-to-the-meeting-request).</span></span>
5. <span data-ttu-id="3dc61-118">[Анна получает ответное сообщение Алены](#step-5-adele-receives-the-response-message).</span><span class="sxs-lookup"><span data-stu-id="3dc61-118">[Adele receives Christie's response message](#step-5-adele-receives-the-response-message).</span></span>
6. <span data-ttu-id="3dc61-119">[Артем проверяет ответы участников в рамках события](#step-6-alex-accesses-responses-as-part-of-the-event).</span><span class="sxs-lookup"><span data-stu-id="3dc61-119">[Alex checks attendees' responses as part of the event](#step-6-alex-accesses-responses-as-part-of-the-event).</span></span>

<span data-ttu-id="3dc61-120">Если Артем предоставил общий доступ, но не делегировал свой календарь Анне:</span><span class="sxs-lookup"><span data-stu-id="3dc61-120">If Alex has shared and not delegated his calendar with Adele:</span></span>

- <span data-ttu-id="3dc61-121">При выполнении входа от имени Анны приложение может [получить календарь, которым Артем поделился с Анной](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span><span class="sxs-lookup"><span data-stu-id="3dc61-121">Signed in as Adele, an app can [get the calendar that Alex has shared with Adele](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span>
- <span data-ttu-id="3dc61-122">Приложение может использовать приглашения и ответы в шагах 2–4 для общего календаря так же, как и для делегированного календаря.</span><span class="sxs-lookup"><span data-stu-id="3dc61-122">The app can use the requests and responses in steps 2 to 4 to apply to the shared calendar the same way as the delegated calendar.</span></span>
- <span data-ttu-id="3dc61-123">На шаге 5 приложение может выполнить вход под именем Артема вместо Анны и получить ответное сообщение Алены. </span><span class="sxs-lookup"><span data-stu-id="3dc61-123">In step 5, the app can sign in as Alex, instead of Adele, to receive Christie's response message.</span></span>

## <a name="step-1-adele-gets-the-delegated-calendar"></a><span data-ttu-id="3dc61-124">Шаг 1. Анна получает делегированный календарь</span><span class="sxs-lookup"><span data-stu-id="3dc61-124">Step 1: Adele gets the delegated calendar</span></span>

<span data-ttu-id="3dc61-125">Войдя в систему под именем Анны, получите календари, к которым у нее есть доступ, и определите, какой календарь делегирован Артемом, чтобы создать в нем событие на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="3dc61-125">Signed in as Adele, get the calendars she has access to and identify the one Alex has delegated to her, so to use it in the next step to create an event in that calendar.</span></span> 

<span data-ttu-id="3dc61-126">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-126">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-127">Воспользуйтесь делегированным разрешением с минимальными правами `Calendars.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-127">Use the least privileged delegated permission, `Calendars.Read.Shared`.</span></span> <span data-ttu-id="3dc61-128">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-128">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="3dc61-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc61-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_Adele_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="3dc61-130">C#</span><span class="sxs-lookup"><span data-stu-id="3dc61-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adele-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc61-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc61-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adele-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc61-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc61-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adele-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dc61-133">Java</span><span class="sxs-lookup"><span data-stu-id="3dc61-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adele-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3dc61-134">Обратите внимание, что успешный отклик включает код ответа HTTP 200, основной календарь Анны, а также копию календаря, делегированного Артемом, в ее почтовом ящике со следующими свойствами:</span><span class="sxs-lookup"><span data-stu-id="3dc61-134">Notice a successful response includes the response code HTTP 200, Adele's own primary calendar, and a copy of the calendar delegated by Alex in Adele's mailbox, with the following properties:</span></span>

- <span data-ttu-id="3dc61-135">**canShare** имеет значение "false", так как Анна является делегатом, а не владельцем календаря.</span><span class="sxs-lookup"><span data-stu-id="3dc61-135">**canShare** is false since Adele is only a delegate and not the calendar owner.</span></span>
- <span data-ttu-id="3dc61-136">**canEdit** имеет значение "true", так как в качестве делегата Анна имеет доступ с правами записи к событиям, не являющимся частными, в делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="3dc61-136">**canEdit** is true since as delegate, Adele has write access to non-private events in the delegated calendar.</span></span>
- <span data-ttu-id="3dc61-137">**owner** имеет значение `Alex Wilber`, которое показывает, что это календарь Артема.</span><span class="sxs-lookup"><span data-stu-id="3dc61-137">**owner** is `Alex Wilber` indicating it is Alex' calendar.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_Adele_calendars",
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
            "id": "AQMkADGkAAAJMjAAAAA==",
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
            "id": "AAMkADRpAABf0JlzAAA=",
            "name": "Alex Wilber",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m4eQ==",
            "canShare": false,
            "canViewPrivateItems": false,
            "canEdit": true,
            "owner": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    ]
}
```

> <span data-ttu-id="3dc61-138">**ПРИМЕЧАНИЕ** Войдя в систему под именем Анны, вы также можете получить делегированный календарь непосредственно из почтового ящика Артема, указав идентификатор Артема и ярлык `calendar` в соответствии с `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-138">**NOTE** Signed in as Adele, you can alternatively get the delegated calendar directly from Alex' mailbox, by specifying Alex' identity and the `calendar` shortcut, as in `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`.</span></span> <span data-ttu-id="3dc61-139">Возвращенный код календаря соответствует почтовому ящику Артема.</span><span class="sxs-lookup"><span data-stu-id="3dc61-139">The returned calendar ID corresponds to only Alex' mailbox.</span></span> 

## <a name="step-2-adele-creates-and-sends-an-invitation-on-alex-behalf"></a><span data-ttu-id="3dc61-140">Шаг 2. Анна создает и отправляет приглашение от имени Артема</span><span class="sxs-lookup"><span data-stu-id="3dc61-140">Step 2: Adele creates and sends an invitation on Alex' behalf</span></span>

<span data-ttu-id="3dc61-141">Войдя в систему под именем Анны, используйте код календаря, полученный на шаге 1, чтобы создать [событие](/graph/api/resources/event) в делегированном календаре и отправить его Алене и Марте от имени Артема.</span><span class="sxs-lookup"><span data-stu-id="3dc61-141">Signed in as Adele, use the calendar ID obtained from step 1 to create an [event](/graph/api/resources/event) in the delegated calendar and send it to Christie and Megan, on Alex' behalf.</span></span>

<span data-ttu-id="3dc61-142">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-142">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-143">Воспользуйтесь делегированным разрешением с минимальными правами `Calendars.ReadWrite.Shared`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-143">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="3dc61-144">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-144">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADRpAABf0JlzAAA="],
  "name": "create_send_invitation"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkADRpAABf0JlzAAA=/events

Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Christmas dinner",
  "body": {
    "contentType": "HTML",
    "content": "Happy holidays!"
  },
  "start": {
      "dateTime": "2019-12-25T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-12-25T22:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Alex' home"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"meganb@contoso.onmicrosoft.com",
        "name": "Megan Bowen"
      },
      "type": "required"
    },
    {
      "emailAddress": {
        "address":"ChristieC@contoso.onmicrosoft.com",
        "name": "Christie Cline"
      },
      "type": "required"
    }
  ]
}
```

<span data-ttu-id="3dc61-145">Обратите внимание, что успешный ответ включает код HTTP 201, а также следующие свойства [события](/graph/api/resources/event):</span><span class="sxs-lookup"><span data-stu-id="3dc61-145">Notice a successful response includes HTTP 201 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3dc61-146">**isOrganizer** имеет значение "true".</span><span class="sxs-lookup"><span data-stu-id="3dc61-146">**isOrganizer** is set to true.</span></span> <span data-ttu-id="3dc61-147">Это свойство обычно имеет значение "true", если владелец календаря (Артем) является организатором собрания.</span><span class="sxs-lookup"><span data-stu-id="3dc61-147">In general, this property is true if the calendar owner (Alex) is the organizer of the meeting.</span></span> <span data-ttu-id="3dc61-148">Это также применимо, если делегат (Анна) организовала собрание от имени владельца. </span><span class="sxs-lookup"><span data-stu-id="3dc61-148">This also applies if a delegate (Adele) organized the meeting on behalf of the owner.</span></span>
- <span data-ttu-id="3dc61-149">В коллекции **attendees** указаны Алена и Марта.</span><span class="sxs-lookup"><span data-stu-id="3dc61-149">The **attendees** collection specifies Megan and Christie.</span></span>
- <span data-ttu-id="3dc61-150">**organizer** имеет значение "Артем", так как приглашение было отправлено делегатом Артема (Анной) для его основного календаря.</span><span class="sxs-lookup"><span data-stu-id="3dc61-150">**organizer** is set to Alex, since the invitation was sent by Alex' delegate (Adele) in Alex' primary calendar.</span></span>
- <span data-ttu-id="3dc61-151">Ни в коллекции **attendees**, ни в свойстве **organizer** не указан делегат (Анна).</span><span class="sxs-lookup"><span data-stu-id="3dc61-151">Neither the **attendees** nor **organizer** specifies the delegate (Adele).</span></span>

<!-- {
  "blockType": "response",
  "name": "create_send_invitation",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars('AAMkADRpAABf0JlzAAA%3D')/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAX8m47Q==\"",
    "id": "AAMkADI4oeRpAABf0LrcAAA=",
    "createdDateTime": "2019-12-21T04:59:01.9766929Z",
    "lastModifiedDateTime": "2019-12-21T04:59:02.0214967Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m47Q==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": false,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI4oeRpAABf0LrcAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-25T18:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-12-25T22:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar"></a><span data-ttu-id="3dc61-152">Шаг 3. Алена получает приглашение на собрание и изучает соответствующее событие в своем календаре</span><span class="sxs-lookup"><span data-stu-id="3dc61-152">Step 3: Christie receives meeting request and inspects the associated event in her calendar</span></span>

<span data-ttu-id="3dc61-153">Доставив приглашение на собрание, Outlook автоматически создает [событие](/graph/api/resources/event) под вопросом в календаре Алены.</span><span class="sxs-lookup"><span data-stu-id="3dc61-153">Upon delivering the meeting request, Outlook automatically creates a tentative [event](/graph/api/resources/event) in Christie's calendar.</span></span>

<span data-ttu-id="3dc61-154">Войдя в систему под именем Алены, получите [eventMessage](/graph/api/resources/eventmessage) и **event**, связанные с приглашением на собрание на шаге 2.</span><span class="sxs-lookup"><span data-stu-id="3dc61-154">Signed in as Christie, get the [eventMessage](/graph/api/resources/eventmessage) and **event** that are associated with the meeting request from step 2.</span></span>

<span data-ttu-id="3dc61-155">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-155">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-156">Воспользуйтесь делегированным разрешением с минимальными правами `Mail.Read` и `Calendar.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-156">Use the least privileged delegated permisson, `Mail.Read` and `Calendar.Read.Shared`.</span></span> <span data-ttu-id="3dc61-157">Дополнительные сведения см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions) и [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-157">For more information, see [mail permissions](permissions-reference.md#mail-permissions) and [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc61-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc61-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5hYdAAA="],
  "name": "get_eventmessage_and_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADADVj3fyAABZ5hYdAAA=?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="3dc61-159">C#</span><span class="sxs-lookup"><span data-stu-id="3dc61-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-and-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc61-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc61-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-and-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc61-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc61-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-and-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dc61-162">Java</span><span class="sxs-lookup"><span data-stu-id="3dc61-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-and-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3dc61-163">Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [eventMessage](/graph/api/resources/eventmessage):</span><span class="sxs-lookup"><span data-stu-id="3dc61-163">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="3dc61-164">**meetingMessageType** определяет это сообщение как `meetingRequest`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-164">**meetingMessageType** specifies this message is `meetingRequest`.</span></span>
- <span data-ttu-id="3dc61-165">**sender** — Анна.</span><span class="sxs-lookup"><span data-stu-id="3dc61-165">**sender** is Adele.</span></span>
- <span data-ttu-id="3dc61-166">**from** — Артем.</span><span class="sxs-lookup"><span data-stu-id="3dc61-166">**from** is Alex.</span></span>
- <span data-ttu-id="3dc61-167">**toRecipients** — Марта и Алена.</span><span class="sxs-lookup"><span data-stu-id="3dc61-167">**toRecipients** include Megan and Christie.</span></span>

<span data-ttu-id="3dc61-168">[Событие](/graph/api/resources/event) имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="3dc61-168">And the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3dc61-169">**attendees** — Артем, Марта и Алена.</span><span class="sxs-lookup"><span data-stu-id="3dc61-169">**attendees** include Alex, Megan, and Christie.</span></span>
- <span data-ttu-id="3dc61-170">**organizer** — Артем.</span><span class="sxs-lookup"><span data-stu-id="3dc61-170">**organizer** is Alex.</span></span>

<span data-ttu-id="3dc61-171">Идентификатор Анны указывается только в свойстве **sender** **eventMessage** и не указывается в связанном с ним **событии**.</span><span class="sxs-lookup"><span data-stu-id="3dc61-171">Adele's identity appears only in the **sender** property of the **eventMessage** and not in the associated **event**.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages(microsoft.graph.eventMessage/event())/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h\"",
    "id": "AAMkADADVj3fyAABZ5hYdAAA=",
    "createdDateTime": "2019-12-21T04:59:03Z",
    "lastModifiedDateTime": "2019-12-21T04:59:04Z",
    "changeKey": "CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h",
    "categories": [],
    "receivedDateTime": "2019-12-21T04:59:03Z",
    "sentDateTime": "2019-12-21T04:59:01Z",
    "hasAttachments": false,
    "internetMessageId": "<DM6PR17MB3593711A1C0A098167F5A977A12C0@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "parentFolderId": "AQMkADIAAAIBDAAAAA==",
    "conversationId": "AAQkADNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADADVj3fyAABZ5hYdAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingRequest",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    },
    "event@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages('AAMkADADVj3fyAABZ5hYdAAA%3D')/microsoft.graph.eventMessage/microsoft.graph.eventMessage/event/$entity",
    "event": {
        "@odata.etag": "W/\"yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==\"",
        "id": "AAMkADADVj3fyAABZ5ieyAAA=",
        "createdDateTime": "2019-12-21T04:59:03.4336242Z",
        "lastModifiedDateTime": "2019-12-27T01:38:32.3766961Z",
        "changeKey": "yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==",
        "categories": [],
        "originalStartTimeZone": "Pacific Standard Time",
        "originalEndTimeZone": "Pacific Standard Time",
        "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
        "reminderMinutesBeforeStart": 15,
        "isReminderOn": true,
        "hasAttachments": false,
        "subject": "Christmas dinner",
        "bodyPreview": "Happy holidays!",
        "importance": "normal",
        "sensitivity": "normal",
        "isAllDay": false,
        "isCancelled": false,
        "isOrganizer": false,
        "responseRequested": true,
        "seriesMasterId": null,
        "showAs": "tentative",
        "type": "singleInstance",
        "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADADVj3fyAABZ5ieyAAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl": null,
        "recurrence": null,
        "responseStatus": {
            "response": "none",
            "time": "2019-12-21T05:16:48.8931825Z"
        },
        "body": {
            "contentType": "html",
            "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
        },
        "start": {
            "dateTime": "2019-12-26T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "end": {
            "dateTime": "2019-12-26T06:00:00.0000000",
            "timeZone": "UTC"
        },
        "location": {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        },
        "locations": [
            {
                "displayName": "Alex' home",
                "locationType": "default",
                "uniqueId": "1396aaf3-e344-4567-a4e3-797557ec24c8",
                "uniqueIdType": "locationStore"
            }
        ],
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Christie Cline",
                    "address": "ChristieC@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
}
```


## <a name="step-4-christie-responds-to-the-meeting-request"></a><span data-ttu-id="3dc61-172">Шаг 4. Алена отвечает на приглашение на собрание</span><span class="sxs-lookup"><span data-stu-id="3dc61-172">Step 4: Christie responds to the meeting request</span></span>

<span data-ttu-id="3dc61-173">Войдя в учетную запись под именем Алены, ответьте на **событие** как "Под вопросом" и включите в отклик ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="3dc61-173">Signed in as Christie, reply to the **event** as tentative, and include a reply message in the response:</span></span>

<span data-ttu-id="3dc61-174">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-174">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-175">Воспользуйтесь делегированным разрешением с минимальными правами `Calendars.ReadWrite.Shared`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-175">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="3dc61-176">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-176">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="3dc61-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc61-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5ieyAAA="],
  "name": "event_reply_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADADVj3fyAABZ5ieyAAA=/tentativelyAccept
Content-type: application/json

{
  "comment": "I will probably be able to make it.",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="3dc61-178">C#</span><span class="sxs-lookup"><span data-stu-id="3dc61-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-reply-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc61-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc61-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-reply-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc61-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc61-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-reply-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dc61-181">Java</span><span class="sxs-lookup"><span data-stu-id="3dc61-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-reply-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3dc61-182">Успешный отклик возвращает код HTTP 202 Принято.</span><span class="sxs-lookup"><span data-stu-id="3dc61-182">A successful response returns HTTP 202 Accepted.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


## <a name="step-5-adele-receives-the-response-message"></a><span data-ttu-id="3dc61-183">Шаг 5. Анна получает ответное сообщение</span><span class="sxs-lookup"><span data-stu-id="3dc61-183">Step 5: Adele receives the response message</span></span>

<span data-ttu-id="3dc61-184">Анна является делегатом для основного календаря Артема, поэтому она получает все ответы на приглашения на собрание для этого календаря от имени Артема.</span><span class="sxs-lookup"><span data-stu-id="3dc61-184">Because Adele is a delegate of Alex' primary calendar, Adele receives all meeting responses for that calendar on Alex' behalf.</span></span>

<span data-ttu-id="3dc61-185">Войдя в систему под именем Анны, получите объект [eventMessage](/graph/api/resources/eventmessage), представляющий ответ Алены на шаге 4.</span><span class="sxs-lookup"><span data-stu-id="3dc61-185">Signed in as Adele, get the [eventMessage](/graph/api/resources/eventmessage) that represents the response from Christie in step 4.</span></span>

<span data-ttu-id="3dc61-186">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-186">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-187">Воспользуйтесь делегированным разрешением с минимальными правами `Mail.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-187">Use the least privileged delegated permission, `Mail.Read.Shared`.</span></span> <span data-ttu-id="3dc61-188">Дополнительные сведения см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-188">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc61-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc61-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI4oeRpAABf0HJUAAA="],
  "name": "message_get_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI4oeRpAABf0HJUAAA=
```
# <a name="c"></a>[<span data-ttu-id="3dc61-190">C#</span><span class="sxs-lookup"><span data-stu-id="3dc61-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc61-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc61-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc61-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc61-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dc61-193">Java</span><span class="sxs-lookup"><span data-stu-id="3dc61-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3dc61-194">Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [eventMessage](/graph/api/resources/eventmessage):</span><span class="sxs-lookup"><span data-stu-id="3dc61-194">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="3dc61-195">**meetingMessageType** имеет значение `meetingTenativelyAccepted`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-195">**meetingMessageType** is `meetingTenativelyAccepted`.</span></span>
- <span data-ttu-id="3dc61-196">**from** — Алена.</span><span class="sxs-lookup"><span data-stu-id="3dc61-196">**from** is Christie.</span></span>
- <span data-ttu-id="3dc61-197">**toRecipients** включает Анну, но не включает владельца календаря, Артема.</span><span class="sxs-lookup"><span data-stu-id="3dc61-197">**toRecipients** includes only Adele, but not the calendar owner Alex.</span></span> <span data-ttu-id="3dc61-198">Это связано с тем, что Артем сохранил значение по умолчанию, позволяющее Outlook направлять все ответы на приглашения на собрание только делегатам.</span><span class="sxs-lookup"><span data-stu-id="3dc61-198">This is because Alex kept the default to have Outlook direct all meeting responses to only delegates.</span></span>

<!-- {
  "blockType": "response",
  "name": "message_get_reply",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/messages/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT\"",
    "id": "AAMkADI4oeRpAABf0HJUAAA=",
    "createdDateTime": "2019-12-21T05:16:55Z",
    "lastModifiedDateTime": "2019-12-21T05:16:57Z",
    "changeKey": "DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT",
    "categories": [],
    "receivedDateTime": "2019-12-21T05:16:56Z",
    "sentDateTime": "2019-12-21T05:16:49Z",
    "hasAttachments": false,
    "internetMessageId": "<86880ccb8ec64184996e46eaddaed279@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Tentative: Christmas dinner",
    "bodyPreview": "I will probably be able to make it.",
    "importance": "normal",
    "parentFolderId": "AQMkAD5GkAAAIBDAAAAA==",
    "conversationId": "AAQkADK25bhNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAwAAoBoZ",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": false,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADI4oeRpAABf0HJUAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingTenativelyAccepted",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nI will probably be able to make it.\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

## <a name="step-6-alex-accesses-responses-as-part-of-the-event"></a><span data-ttu-id="3dc61-199">Шаг 6. Артем получает доступ к ответам в рамках события</span><span class="sxs-lookup"><span data-stu-id="3dc61-199">Step 6: Alex accesses responses as part of the event</span></span>

<span data-ttu-id="3dc61-200">Артем сохранил значение по умолчанию, позволяющее Outlook направлять все приглашения на собрание и ответы только делегатам, поэтому он не получает ответ Алены на шаге 4.</span><span class="sxs-lookup"><span data-stu-id="3dc61-200">Because Alex kept the default to have Outlook direct all meeting requests and responses to only delegates, Alex does not receive Christie's response from step 4.</span></span> <span data-ttu-id="3dc61-201">Однако он может получить ответ с помощью [события](/graph/api/resources/event) в своем основном календаре.</span><span class="sxs-lookup"><span data-stu-id="3dc61-201">He can however get the response through the [event](/graph/api/resources/event) in his primary calendar.</span></span>

<span data-ttu-id="3dc61-202">Войдя в систему под именем Артема, получите [событие](/graph/api/resources/event), созданное Анной на шаге 2, а также отклики свойства **attendees**.</span><span class="sxs-lookup"><span data-stu-id="3dc61-202">Signed in as Alex, get the [event](/graph/api/resources/event) that Adele created in step 2 and get responses from the **attendees** property.</span></span>

<span data-ttu-id="3dc61-203">**Разрешения Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="3dc61-203">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3dc61-204">Воспользуйтесь делегированным разрешением с минимальными правами `Calendars.Read`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-204">Use the least privileged delegated permission, `Calendars.Read`.</span></span> <span data-ttu-id="3dc61-205">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="3dc61-205">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc61-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc61-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADJXJGu0AABf02qwAAA="],
  "name": "event_get_responses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=
```
# <a name="c"></a>[<span data-ttu-id="3dc61-207">C#</span><span class="sxs-lookup"><span data-stu-id="3dc61-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-responses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc61-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc61-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-responses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc61-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc61-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-responses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dc61-210">Java</span><span class="sxs-lookup"><span data-stu-id="3dc61-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-responses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3dc61-211">Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [события](/graph/api/resources/event):</span><span class="sxs-lookup"><span data-stu-id="3dc61-211">Notice a successful response includes the response code HTTP 200 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3dc61-212">**isOrganizer** имеет значение "true".</span><span class="sxs-lookup"><span data-stu-id="3dc61-212">**isOrganizer** is true.</span></span>
- <span data-ttu-id="3dc61-213">**attendees** — только Марта и Алена.</span><span class="sxs-lookup"><span data-stu-id="3dc61-213">**attendees** include only Megan and Christie.</span></span>
- <span data-ttu-id="3dc61-214">В свойстве **status** каждого экземпляра **attendee** указан ответ участника.</span><span class="sxs-lookup"><span data-stu-id="3dc61-214">The **status** property of each **attendee** instance indicates any response from the attendee:</span></span>
  - <span data-ttu-id="3dc61-215">Ответ Марты — `none`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-215">Megan's response is `none`.</span></span>
  - <span data-ttu-id="3dc61-216">Ответ Алены — `tentativelyAccepted`.</span><span class="sxs-lookup"><span data-stu-id="3dc61-216">Christie's response is `tentativelyAccepted`.</span></span>
- <span data-ttu-id="3dc61-217">**organizer** — Артем.</span><span class="sxs-lookup"><span data-stu-id="3dc61-217">**organizer** is Alex.</span></span>
- <span data-ttu-id="3dc61-218">В свойствах возвращенного **события** не указывается делегат, Анна.</span><span class="sxs-lookup"><span data-stu-id="3dc61-218">No property in the returned **event** indicates the delegate, Adele.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_get_responses",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AQMkADAw7QAAAJfygAAAA%3D%3D')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==\"",
    "id": "AAMkADJXJGu0AABf02qwAAA=",
    "createdDateTime": "2019-12-21T04:59:01.4435895Z",
    "lastModifiedDateTime": "2019-12-21T05:16:54.689345Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADJXJGu0AABf02qwAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-26T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-12-26T06:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "tentativelyAccepted",
                "time": "2019-12-21T05:16:48.8931825Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="next-steps"></a><span data-ttu-id="3dc61-219">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3dc61-219">Next steps</span></span>

<span data-ttu-id="3dc61-220">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="3dc61-220">Find out more about:</span></span>

- [<span data-ttu-id="3dc61-221">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="3dc61-221">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="3dc61-222">Предоставление общего доступа к календарю или его делегирование в Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3dc61-222">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="3dc61-223">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="3dc61-223">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="3dc61-224">[API календаря](/graph/api/resources/calendar) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="3dc61-224">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph v1.0.</span></span>
