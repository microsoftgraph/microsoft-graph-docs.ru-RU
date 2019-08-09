---
title: Создание события
description: С помощью этого API можно создать событие в календаре по умолчанию или указанном календаре.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 559c37348bd2b594e191ba04faf0668198c6e4dc
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245677"
---
# <a name="create-event"></a><span data-ttu-id="c1105-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="c1105-103">Create event</span></span>

<span data-ttu-id="c1105-104">Создайте новое событие в календаре с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="c1105-104">Use this API to create a new Calendar in a calendar group.</span></span> <span data-ttu-id="c1105-105">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="c1105-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c1105-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1105-106">Permissions</span></span>
<span data-ttu-id="c1105-107">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="c1105-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1105-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1105-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1105-109">Календарь</span><span class="sxs-lookup"><span data-stu-id="c1105-109">Calendar</span></span> | <span data-ttu-id="c1105-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1105-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1105-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1105-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1105-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1105-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="c1105-113">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="c1105-113">user calendar</span></span> | <span data-ttu-id="c1105-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1105-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="c1105-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1105-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="c1105-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1105-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="c1105-117">календарь группы</span><span class="sxs-lookup"><span data-stu-id="c1105-117">group calendar</span></span> | <span data-ttu-id="c1105-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1105-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="c1105-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1105-119">Not supported.</span></span> | <span data-ttu-id="c1105-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1105-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1105-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1105-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c1105-122">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c1105-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="c1105-123">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c1105-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="c1105-124">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c1105-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="c1105-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1105-125">Request headers</span></span>
| <span data-ttu-id="c1105-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1105-126">Header</span></span>       | <span data-ttu-id="c1105-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c1105-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1105-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1105-128">Authorization</span></span>  | <span data-ttu-id="c1105-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1105-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1105-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1105-131">Content-Type</span></span>  | <span data-ttu-id="c1105-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1105-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1105-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1105-134">Request body</span></span>
<span data-ttu-id="c1105-135">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1105-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c1105-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1105-136">Response</span></span>

<span data-ttu-id="c1105-137">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c1105-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1105-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c1105-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1105-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1105-139">Request</span></span>
<span data-ttu-id="c1105-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1105-140">Here is an example of the request.</span></span>
<span data-ttu-id="c1105-141">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1105-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1105-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1105-142">--Http</span></span>](#tab/http)
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
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1105-143">C#</span><span class="sxs-lookup"><span data-stu-id="c1105-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1105-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1105-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1105-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1105-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1105-146">Java</span><span class="sxs-lookup"><span data-stu-id="c1105-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1105-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1105-147">Response</span></span>
<span data-ttu-id="c1105-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1105-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
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
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
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
