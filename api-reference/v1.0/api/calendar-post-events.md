---
title: Создание события
description: С помощью этого API можно создать событие в календаре по умолчанию или указанном календаре.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe894ed0ceb5cdeceadcc615503b0993f64c1c17
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434883"
---
# <a name="create-event"></a><span data-ttu-id="a4459-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="a4459-103">Create event</span></span>

<span data-ttu-id="a4459-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4459-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4459-105">Создайте новое событие в календаре с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="a4459-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="a4459-106">Это может быть календарь для [пользователя](../resources/user.md) или стандартный календарь для [группы](../resources/group.md) Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4459-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a4459-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4459-107">Permissions</span></span>
<span data-ttu-id="a4459-108">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="a4459-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a4459-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4459-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4459-110">Календарь</span><span class="sxs-lookup"><span data-stu-id="a4459-110">Calendar</span></span> | <span data-ttu-id="a4459-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4459-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4459-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4459-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4459-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4459-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="a4459-114">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="a4459-114">user calendar</span></span> | <span data-ttu-id="a4459-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4459-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="a4459-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4459-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="a4459-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4459-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="a4459-118">календарь группы</span><span class="sxs-lookup"><span data-stu-id="a4459-118">group calendar</span></span> | <span data-ttu-id="a4459-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4459-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="a4459-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4459-120">Not supported.</span></span> | <span data-ttu-id="a4459-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4459-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4459-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4459-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a4459-123">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4459-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="a4459-124">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="a4459-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
<span data-ttu-id="a4459-125">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="a4459-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="a4459-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4459-126">Request headers</span></span>
| <span data-ttu-id="a4459-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4459-127">Header</span></span>       | <span data-ttu-id="a4459-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a4459-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4459-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4459-129">Authorization</span></span>  | <span data-ttu-id="a4459-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4459-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4459-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4459-132">Content-Type</span></span>  | <span data-ttu-id="a4459-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4459-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4459-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4459-135">Request body</span></span>
<span data-ttu-id="a4459-136">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4459-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4459-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4459-137">Response</span></span>

<span data-ttu-id="a4459-138">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4459-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4459-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4459-139">Examples</span></span>

### <a name="example-1-create-an-event-in-a-specific-calendar"></a><span data-ttu-id="a4459-140">Пример 1. Создание события в определенном календаре</span><span class="sxs-lookup"><span data-stu-id="a4459-140">Example 1: Create an event in a specific calendar</span></span>

#### <a name="request"></a><span data-ttu-id="a4459-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4459-141">Request</span></span>
<span data-ttu-id="a4459-142">В примере ниже создается событие в определенном календаре и событию назначается необязательное значение **transactionId**.</span><span class="sxs-lookup"><span data-stu-id="a4459-142">The following example creates an event in a specific calendar and assigns the event an optional **transactionId** value.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4459-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4459-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="a4459-144">C#</span><span class="sxs-lookup"><span data-stu-id="a4459-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4459-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4459-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4459-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4459-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4459-147">Java</span><span class="sxs-lookup"><span data-stu-id="a4459-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4459-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4459-148">Response</span></span>
<span data-ttu-id="a4459-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4459-149">Here is an example of the response.</span></span> 

><span data-ttu-id="a4459-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4459-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
}-->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "hideAttendees": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider": "unknown",
    "onlineMeeting": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
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
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```
### <a name="example-2-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="a4459-151">Пример 2. Создание и включение события в качестве собрания по сети</span><span class="sxs-lookup"><span data-stu-id="a4459-151">Example 2: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="a4459-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4459-152">Request</span></span>
<span data-ttu-id="a4459-153">В следующем примере создается событие в указанном календаре пользователя, вошедшего в систему, и оно включается в виде онлайн-собрания.</span><span class="sxs-lookup"><span data-stu-id="a4459-153">The following example creates an event in the specified calendar of the signed-in user's and enables it as an online meeting.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4459-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4459-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU9zAAAAAGtlAAA="],
  "name": "create_event_from_calendar_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU9zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="a4459-155">C#</span><span class="sxs-lookup"><span data-stu-id="a4459-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4459-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4459-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4459-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4459-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4459-158">Java</span><span class="sxs-lookup"><span data-stu-id="a4459-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-with-online-meeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4459-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4459-159">Response</span></span>
<span data-ttu-id="a4459-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4459-160">Here is an example of the response.</span></span> 

><span data-ttu-id="a4459-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4459-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_event_from_calendar_with_online_meeting",
  "@odata.type": "microsoft.graph.event"
}-->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU9zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "hideAttendees": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
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
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

