---
title: Создание события
description: Создайте событие в календаре пользователя по умолчанию или указанном календаре.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fe9864474a83a827430b539d80127441b548ecb1
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805097"
---
# <a name="create-event"></a><span data-ttu-id="fbec9-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="fbec9-103">Create Event</span></span>

<span data-ttu-id="fbec9-104">Создайте [событие](../resources/event.md) в календаре пользователя по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="fbec9-104">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="fbec9-105">В рамках этих значений вы можете задать часовой пояс для каждого времени начала или окончания события, так как свойства **start** и **end** относятся к типу [dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="fbec9-105">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="fbec9-106">Сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="fbec9-106">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="fbec9-107">При отправке события сервер отправляет приглашения всем участникам.</span><span class="sxs-lookup"><span data-stu-id="fbec9-107">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="fbec9-108">**Установка места проведения события**</span><span class="sxs-lookup"><span data-stu-id="fbec9-108">**Setting the location in an event**</span></span>

<span data-ttu-id="fbec9-109">Администратор Exchange может настроить почтовый ящик и адрес электронной почты для ресурса, например конференц-зала, или оборудования, например проектора.</span><span class="sxs-lookup"><span data-stu-id="fbec9-109">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="fbec9-110">Затем пользователи могут пригласить ресурс в качестве участников собрания.</span><span class="sxs-lookup"><span data-stu-id="fbec9-110">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="fbec9-111">Сервер принимает или отклоняет приглашение на собрание от имени ресурса, руководствуясь расписанием его занятости.</span><span class="sxs-lookup"><span data-stu-id="fbec9-111">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="fbec9-112">Если сервер принимает приглашение от имени ресурса, он создает соответствующее событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="fbec9-112">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="fbec9-113">В случае переноса собрания сервер автоматически обновляет событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="fbec9-113">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="fbec9-114">Еще одно преимущество настройки почтового ящика для ресурса — возможность управления расписанием для ресурса. Например, вы можете разрешить бронирование частного конференц-зала только руководителям и их представителям.</span><span class="sxs-lookup"><span data-stu-id="fbec9-114">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="fbec9-115">Если вы организуете событие, у которого есть место проведения:</span><span class="sxs-lookup"><span data-stu-id="fbec9-115">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="fbec9-116">Задайте соответствующее значение для свойства **location** объекта **event**.</span><span class="sxs-lookup"><span data-stu-id="fbec9-116">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="fbec9-117">Задайте необязательное свойство **locationEmailAddress**, если у места проведения собрания есть адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fbec9-117">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="fbec9-118">Кроме того, если место проведения собрания было настроено как ресурс или для мероприятия требуется какое-либо оборудование, настроенное как ресурс:</span><span class="sxs-lookup"><span data-stu-id="fbec9-118">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="fbec9-119">Пригласите ресурс как объект [attendee](../resources/attendee.md).</span><span class="sxs-lookup"><span data-stu-id="fbec9-119">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="fbec9-120">Задайте для свойства **type** участника значение `resource`.</span><span class="sxs-lookup"><span data-stu-id="fbec9-120">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="fbec9-121">Укажите свойство **emailAddress** участника в качестве электронного адреса ресурса.</span><span class="sxs-lookup"><span data-stu-id="fbec9-121">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="fbec9-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbec9-122">Permissions</span></span>
<span data-ttu-id="fbec9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbec9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbec9-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbec9-125">Permission type</span></span>      | <span data-ttu-id="fbec9-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbec9-126">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbec9-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbec9-127">Delegated (work or school account)</span></span> | <span data-ttu-id="fbec9-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbec9-128">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fbec9-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbec9-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbec9-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbec9-130">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fbec9-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbec9-131">Application</span></span> | <span data-ttu-id="fbec9-132">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbec9-132">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbec9-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbec9-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="fbec9-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbec9-134">Request headers</span></span>
| <span data-ttu-id="fbec9-135">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbec9-135">Header</span></span>       | <span data-ttu-id="fbec9-136">Значение</span><span class="sxs-lookup"><span data-stu-id="fbec9-136">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="fbec9-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbec9-137">Authorization</span></span>  | <span data-ttu-id="fbec9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbec9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fbec9-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbec9-140">Content-Type</span></span>  | <span data-ttu-id="fbec9-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbec9-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbec9-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbec9-143">Request body</span></span>
<span data-ttu-id="fbec9-144">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbec9-144">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="fbec9-145">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="fbec9-145">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="fbec9-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbec9-146">Response</span></span>

<span data-ttu-id="fbec9-147">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fbec9-147">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbec9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="fbec9-148">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fbec9-149">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="fbec9-149">Request 1</span></span>
<span data-ttu-id="fbec9-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbec9-150">Here is an example of the request.</span></span> <span data-ttu-id="fbec9-151">Использует заголовок запроса `Prefer: outlook.timezone`, чтобы указать часовой пояс для параметров времени **start** и **end** в отклике.</span><span class="sxs-lookup"><span data-stu-id="fbec9-151">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fbec9-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbec9-152">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
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
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fbec9-153">C#</span><span class="sxs-lookup"><span data-stu-id="fbec9-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbec9-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbec9-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fbec9-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbec9-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fbec9-156">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbec9-156">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="fbec9-157">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="fbec9-157">Response 1</span></span>
<span data-ttu-id="fbec9-158">Ниже приведен пример ответа, где показано, что свойства **start** и **end** соответствуют часовому поясу, указанному в заголовке `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="fbec9-158">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="fbec9-159">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fbec9-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbec9-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbec9-160">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
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


##### <a name="request-2"></a><span data-ttu-id="fbec9-161">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="fbec9-161">Request 2</span></span>
<span data-ttu-id="fbec9-162">В следующем примере задаются 3 расположения, где организатор и участники могут посетить мероприятие.</span><span class="sxs-lookup"><span data-stu-id="fbec9-162">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="fbec9-163">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbec9-163">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fbec9-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbec9-164">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
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
  ]

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fbec9-165">C#</span><span class="sxs-lookup"><span data-stu-id="fbec9-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbec9-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbec9-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fbec9-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbec9-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="fbec9-168">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="fbec9-168">Response 2</span></span>
<span data-ttu-id="fbec9-169">В приведенном ниже примере ответа показано созданное событие, в котором указаны сведения о 3 местах проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="fbec9-169">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="fbec9-170">Так как используется заголовок запроса `Prefer: outlook.timezone="Pacific Standard Time"`, свойства **start** и **end** выражены в формате PST.</span><span class="sxs-lookup"><span data-stu-id="fbec9-170">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="fbec9-171">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fbec9-171">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbec9-172">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbec9-172">All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "iCalUId":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
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


##### <a name="request-3"></a><span data-ttu-id="fbec9-173">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="fbec9-173">Request 3</span></span>
<span data-ttu-id="fbec9-174">В третьем примере показано, как создать повторяющееся событие.</span><span class="sxs-lookup"><span data-stu-id="fbec9-174">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="fbec9-175">Событие происходит с 12:00 до 14:00 каждый понедельник с 4 сентября 2017 г. до конца года.</span><span class="sxs-lookup"><span data-stu-id="fbec9-175">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fbec9-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbec9-176">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fbec9-177">C#</span><span class="sxs-lookup"><span data-stu-id="fbec9-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbec9-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbec9-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fbec9-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbec9-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fbec9-180">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbec9-180">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="fbec9-181">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="fbec9-181">Response 3</span></span>
<span data-ttu-id="fbec9-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fbec9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
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


## <a name="see-also"></a><span data-ttu-id="fbec9-185">См. также</span><span class="sxs-lookup"><span data-stu-id="fbec9-185">See also</span></span>

- [<span data-ttu-id="fbec9-186">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fbec9-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fbec9-187">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="fbec9-187">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fbec9-188">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="fbec9-188">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
