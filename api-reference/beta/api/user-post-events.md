---
title: Создание события
description: Создайте событие в календаре пользователя по умолчанию или указанном календаре.
localization_priority: Normal
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: cad97bd555d6d0388f6f402f1365a152942af34b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049627"
---
# <a name="create-event"></a><span data-ttu-id="30a2d-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="30a2d-103">Create Event</span></span>

<span data-ttu-id="30a2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a2d-105">Создайте [событие](../resources/event.md) в календаре пользователя по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="30a2d-105">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="30a2d-106">По умолчанию при создании события для свойства **allowNewTimeProposals** устанавливается значение true. Это означает, что приглашенные могут предлагать другое время и дату события.</span><span class="sxs-lookup"><span data-stu-id="30a2d-106">By default, the **allowNewTimeProposals** property is set to true when an event is created, which means invitees can propose a different date/time for the event.</span></span> <span data-ttu-id="30a2d-107">Дополнительные сведения о том, как предлагать время, а также получать и принимать новое предложенное время, см. в статье [Предложение нового времени собрания](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="30a2d-107">See [Propose new meeting times](/graph/outlook-calendar-meeting-proposals) for more information on how to propose a time, and how to receive and accept a new time proposal.</span></span>

<span data-ttu-id="30a2d-108">В рамках этих значений вы можете задать часовой пояс для каждого времени начала или окончания события, так как свойства **start** и **end** относятся к типу [dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="30a2d-108">You can specify the time zone for each of the start and end times of the event as part of their values, because the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="30a2d-109">Сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="30a2d-109">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="30a2d-110">При отправке события сервер отправляет приглашения всем участникам.</span><span class="sxs-lookup"><span data-stu-id="30a2d-110">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="30a2d-111">**Установка места проведения события**</span><span class="sxs-lookup"><span data-stu-id="30a2d-111">**Setting the location in an event**</span></span>

<span data-ttu-id="30a2d-112">Администратор Exchange может настроить почтовый ящик и адрес электронной почты для ресурса, например конференц-зала, или оборудования, например проектора.</span><span class="sxs-lookup"><span data-stu-id="30a2d-112">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="30a2d-113">Затем пользователи могут пригласить ресурс в качестве участников собрания.</span><span class="sxs-lookup"><span data-stu-id="30a2d-113">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="30a2d-114">Сервер принимает или отклоняет приглашение на собрание от имени ресурса, руководствуясь расписанием его занятости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-114">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span>
<span data-ttu-id="30a2d-115">Если сервер принимает приглашение от имени ресурса, он создает соответствующее событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="30a2d-115">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="30a2d-116">В случае переноса собрания сервер автоматически обновляет событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="30a2d-116">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="30a2d-117">Еще одно преимущество настройки почтового ящика для ресурса — возможность управления расписанием для ресурса. Например, вы можете разрешить бронирование частного конференц-зала только руководителям и их представителям.</span><span class="sxs-lookup"><span data-stu-id="30a2d-117">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="30a2d-118">Если вы организуете событие, у которого есть место проведения:</span><span class="sxs-lookup"><span data-stu-id="30a2d-118">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="30a2d-119">Задайте соответствующее значение для свойства **location** объекта **event**.</span><span class="sxs-lookup"><span data-stu-id="30a2d-119">Set the **location** property of the **event** accordingly.</span></span>
2. <span data-ttu-id="30a2d-120">Задайте необязательное свойство **locationEmailAddress**, если у места проведения собрания есть адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a2d-120">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="30a2d-121">Кроме того, если место проведения собрания было настроено как ресурс или для мероприятия требуется какое-либо оборудование, настроенное как ресурс:</span><span class="sxs-lookup"><span data-stu-id="30a2d-121">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="30a2d-122">Пригласите ресурс как объект [attendee](../resources/attendee.md).</span><span class="sxs-lookup"><span data-stu-id="30a2d-122">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="30a2d-123">Задайте для свойства **type** участника значение `resource`.</span><span class="sxs-lookup"><span data-stu-id="30a2d-123">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="30a2d-124">Укажите свойство **emailAddress** участника в качестве электронного адреса ресурса.</span><span class="sxs-lookup"><span data-stu-id="30a2d-124">Set the attendee **emailAddress** as the resource email address.</span></span>


## <a name="permissions"></a><span data-ttu-id="30a2d-125">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30a2d-125">Permissions</span></span>
<span data-ttu-id="30a2d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a2d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a2d-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30a2d-128">Permission type</span></span>      | <span data-ttu-id="30a2d-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30a2d-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30a2d-130">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30a2d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="30a2d-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a2d-131">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="30a2d-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30a2d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a2d-133">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a2d-133">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="30a2d-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30a2d-134">Application</span></span> | <span data-ttu-id="30a2d-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a2d-135">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30a2d-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="30a2d-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30a2d-137">Request headers</span></span>
| <span data-ttu-id="30a2d-138">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30a2d-138">Header</span></span>       | <span data-ttu-id="30a2d-139">Значение</span><span class="sxs-lookup"><span data-stu-id="30a2d-139">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="30a2d-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30a2d-140">Authorization</span></span>  | <span data-ttu-id="30a2d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a2d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="30a2d-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30a2d-143">Content-Type</span></span>  | <span data-ttu-id="30a2d-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a2d-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30a2d-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30a2d-146">Request body</span></span>
<span data-ttu-id="30a2d-147">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-147">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="30a2d-148">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="30a2d-148">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="30a2d-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="30a2d-149">Response</span></span>

<span data-ttu-id="30a2d-150">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="30a2d-150">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30a2d-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="30a2d-151">Examples</span></span>

### <a name="example-1-create-an-event-in-the-specified-time-zone-and-assign-the-event-an-optional-transactionid-value"></a><span data-ttu-id="30a2d-152">Пример 1. Создание события в указанном часовом поясе и назначение события необязательным значением transactionId</span><span class="sxs-lookup"><span data-stu-id="30a2d-152">Example 1: Create an event in the specified time zone, and assign the event an optional transactionId value</span></span>

#### <a name="request"></a><span data-ttu-id="30a2d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-153">Request</span></span>
<span data-ttu-id="30a2d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30a2d-154">Here is an example of the request.</span></span> <span data-ttu-id="30a2d-155">В нем используется заголовок запроса `Prefer: outlook.timezone`, чтобы указать часовой пояс для параметров времени начала и окончания в отклике.</span><span class="sxs-lookup"><span data-stu-id="30a2d-155">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the start and end times in the response.</span></span> <span data-ttu-id="30a2d-156">Он также настраивает свойство transactionId, чтобы сократить количество ненужных повторных попыток на сервере.</span><span class="sxs-lookup"><span data-stu-id="30a2d-156">It also sets the transactionId property to reduce unnecessary retries on the server.</span></span>

# <a name="http"></a>[<span data-ttu-id="30a2d-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a2d-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="30a2d-158">C#</span><span class="sxs-lookup"><span data-stu-id="30a2d-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a2d-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a2d-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a2d-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a2d-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a2d-161">Java</span><span class="sxs-lookup"><span data-stu-id="30a2d-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="30a2d-162">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-162">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="30a2d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2d-163">Response</span></span>
<span data-ttu-id="30a2d-164">Ниже приведен пример ответа, где показано, что свойства **start** и **end** соответствуют часовому поясу, указанному в заголовке `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="30a2d-164">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="30a2d-165">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-165">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```


### <a name="example-2-create-an-event-that-occurs-in-multiple-locations"></a><span data-ttu-id="30a2d-166">Пример 2. Создание события, которое происходит в нескольких местах</span><span class="sxs-lookup"><span data-stu-id="30a2d-166">Example 2: Create an event that occurs in multiple locations</span></span>

#### <a name="request"></a><span data-ttu-id="30a2d-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-167">Request</span></span>
<span data-ttu-id="30a2d-168">В следующем примере задаются 3 расположения, где организатор и участники могут посетить мероприятие.</span><span class="sxs-lookup"><span data-stu-id="30a2d-168">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="30a2d-169">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-169">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="30a2d-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a2d-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 1390

{
  "subject": "Plan summer company picnic",
  "body": {
    "contentType": "HTML",
    "content": "Let's kick-start this event planning!"
  },
  "start": {
      "dateTime": "2017-08-30T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-08-30T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "DanaS@contoso.onmicrosoft.com",
        "name": "Dana Swope"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "AlexW@contoso.onmicrosoft.com",
        "name": "Alex Wilber"
      },
      "type": "Required"
    }
  ],
  "location": {
    "displayName": "Conf Room 3; Fourth Coffee; Home Office",
    "locationType": "Default"
  },
  "locations": [
    {
      "displayName": "Conf Room 3"
    },
    {
      "displayName": "Fourth Coffee",
      "address": {
        "street": "4567 Main St",
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "US",
        "postalCode": "32008"
      },
      "coordinates": {
        "latitude": 47.672,
        "longitude": -102.103
      }
    },
    {
      "displayName": "Home Office"
    }
  ],
  "allowNewTimeProposals": true
}
```
# <a name="c"></a>[<span data-ttu-id="30a2d-171">C#</span><span class="sxs-lookup"><span data-stu-id="30a2d-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a2d-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a2d-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a2d-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a2d-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a2d-174">Java</span><span class="sxs-lookup"><span data-stu-id="30a2d-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="30a2d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2d-175">Response</span></span>
<span data-ttu-id="30a2d-176">В приведенном ниже примере ответа показано созданное событие, в котором указаны сведения о 3 местах проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="30a2d-176">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="30a2d-177">Так как используется заголовок запроса `Prefer: outlook.timezone="Pacific Standard Time"`, свойства **start** и **end** выражены в формате PST.</span><span class="sxs-lookup"><span data-stu-id="30a2d-177">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="30a2d-178">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-178">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2985

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "uid":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "hideAttendees": false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isDraft": false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
  "isOnlineMeeting":true,
  "onlineMeetingProvider":"unknown",
  "onlineMeeting":null,
  "allowNewTimeProposals": true,
  "responseStatus":{
    "response":"organizer",
    "time":"0001-01-01T00:00:00Z"
  },
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "recurrence":null,
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```


### <a name="example-3-create-a-weekly-recurring-event"></a><span data-ttu-id="30a2d-179">Пример 3. Создание еженедельно повторяющегося события</span><span class="sxs-lookup"><span data-stu-id="30a2d-179">Example 3: Create a weekly recurring event</span></span>

#### <a name="request"></a><span data-ttu-id="30a2d-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-180">Request</span></span>
<span data-ttu-id="30a2d-181">В третьем примере показано, как создать событие, повторяющееся раз в неделю.</span><span class="sxs-lookup"><span data-stu-id="30a2d-181">The third example shows how to create a recurring event that occurs once a week.</span></span> <span data-ttu-id="30a2d-182">Событие происходит с 12:00 до 14:00 каждый понедельник с 4 сентября 2017 г. до конца года.</span><span class="sxs-lookup"><span data-stu-id="30a2d-182">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="http"></a>[<span data-ttu-id="30a2d-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a2d-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon time work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="30a2d-184">C#</span><span class="sxs-lookup"><span data-stu-id="30a2d-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a2d-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a2d-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a2d-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a2d-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a2d-187">Java</span><span class="sxs-lookup"><span data-stu-id="30a2d-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-recurring-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="30a2d-188">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-188">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="30a2d-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2d-189">Response</span></span>
<span data-ttu-id="30a2d-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30a2d-190">Here is an example of the response.</span></span>
<span data-ttu-id="30a2d-191">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-191">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting":true,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T14:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar",
        "locationType":"default",
        "uniqueId":"Harry's Bar",
        "uniqueIdType":"private"
    },
    "locations":[
        {
            "displayName":"Harry's Bar",
            "locationType":"default",
            "uniqueIdType":"unknown"
        }
    ],
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    },
    "OnlineMeeting":null
}
```

### <a name="example-4-create-a-daily-recurring-event"></a><span data-ttu-id="30a2d-192">Пример 4. Создание ежедневного повторяющегося события</span><span class="sxs-lookup"><span data-stu-id="30a2d-192">Example 4: Create a daily recurring event</span></span>

#### <a name="request"></a><span data-ttu-id="30a2d-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-193">Request</span></span>
<span data-ttu-id="30a2d-194">В четвертом примере показано, как создать событие, повторяющееся ежедневно.</span><span class="sxs-lookup"><span data-stu-id="30a2d-194">The fourth example shows how to create a daily recurring event.</span></span> <span data-ttu-id="30a2d-195">Событие происходит с 12:00 до 14:00 каждый день, начиная с 25 февраля 2020 г., в течение двух случаев.</span><span class="sxs-lookup"><span data-stu-id="30a2d-195">The event occurs from 12:00pm to 2:00pm, every day starting February 25, 2020, for two occurrences.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_event_recurring_daily"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2020-02-25T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2020-02-25T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AlexW@contoso.OnMicrosoft.com",
        "name": "Alex Wilbur"
      },
      "type": "required"
    }
  ],
  "recurrence": {
    "pattern": {
      "type": "daily",
      "interval": 1
    },
    "range": {
      "type": "numbered",
      "startDate": "2020-02-25",
      "numberOfOccurrences": 2
    }
  }
}
```


<span data-ttu-id="30a2d-196">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-196">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="30a2d-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2d-197">Response</span></span>
<span data-ttu-id="30a2d-198">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30a2d-198">Here is an example of the response.</span></span>
<span data-ttu-id="30a2d-199">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-199">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring_daily",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendar/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAhrvLSg==\"",
    "id": "AAMkADU5NWAAA=",
    "createdDateTime": "2020-02-18T22:13:47.2967773Z",
    "lastModifiedDateTime": "2020-02-18T22:13:47.7398267Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAhrvLSg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E0080000000027B6D5B0A8E6D50100000000000000001000000065CD4D206C79D44CBF53D42B6E79CE55",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "hideAttendees": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does noon work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADU5NWAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider": "unknown",
    "allowNewTimeProposals": true,
    "onlineMeeting": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes noon work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2020-02-25T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2020-02-25T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "recurrence": {
        "pattern": {
            "type": "daily",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "numbered",
            "startDate": "2020-02-25",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Pacific Standard Time",
            "numberOfOccurrences": 2
        }
    },
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
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    }
}
```


### <a name="example-5-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="30a2d-200">Пример 5. Создание и включить событие в качестве собрания в Интернете</span><span class="sxs-lookup"><span data-stu-id="30a2d-200">Example 5: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="30a2d-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2d-201">Request</span></span>
<span data-ttu-id="30a2d-202">Вот пример запроса, который создает событие и включает его в качестве онлайн-встречи.</span><span class="sxs-lookup"><span data-stu-id="30a2d-202">Here is an example of a request which creates an event and enables it as an online meeting.</span></span> <span data-ttu-id="30a2d-203">Использует заголовок запроса `Prefer: outlook.timezone`, чтобы указать часовой пояс для параметров времени **start** и **end** в отклике.</span><span class="sxs-lookup"><span data-stu-id="30a2d-203">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="30a2d-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a2d-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="30a2d-205">C#</span><span class="sxs-lookup"><span data-stu-id="30a2d-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a2d-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a2d-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a2d-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a2d-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a2d-208">Java</span><span class="sxs-lookup"><span data-stu-id="30a2d-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-with-online-meeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="30a2d-209">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a2d-209">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="30a2d-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2d-210">Response</span></span>
<span data-ttu-id="30a2d-211">Ниже приведен пример ответа, где показано, что свойства **start** и **end** соответствуют часовому поясу, указанному в заголовке `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="30a2d-211">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="30a2d-212">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30a2d-212">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_with_online_meeting",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt8AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```



## <a name="see-also"></a><span data-ttu-id="30a2d-213">См. также</span><span class="sxs-lookup"><span data-stu-id="30a2d-213">See also</span></span>

- [<span data-ttu-id="30a2d-214">Планирование повторных встреч, как повторяющихся событий в Outlook</span><span class="sxs-lookup"><span data-stu-id="30a2d-214">Schedule repeating appointments as recurring events in Outlook</span></span>](/graph/outlook-schedule-recurring-events)
- [<span data-ttu-id="30a2d-215">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="30a2d-215">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="30a2d-216">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="30a2d-216">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="30a2d-217">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="30a2d-217">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


