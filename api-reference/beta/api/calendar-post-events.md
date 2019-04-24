---
title: Создание события
description: С помощью этого API можно создать событие в календаре по умолчанию или указанном календаре.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: c620b2fb25a0ead99a07304b61db314300f6ea2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462083"
---
# <a name="create-event"></a><span data-ttu-id="89812-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="89812-103">Create event</span></span>

<span data-ttu-id="89812-104">С помощью этого API можно создать событие в календаре по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="89812-104">Use this API to create a new event in the default or specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="89812-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89812-105">Permissions</span></span>
<span data-ttu-id="89812-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89812-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89812-108">Permission type</span></span>      | <span data-ttu-id="89812-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89812-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89812-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89812-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89812-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89812-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="89812-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89812-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89812-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89812-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="89812-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89812-114">Application</span></span> | <span data-ttu-id="89812-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89812-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="89812-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89812-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="89812-117">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="89812-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="89812-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="89812-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="89812-119">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="89812-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="89812-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89812-120">Request headers</span></span>
| <span data-ttu-id="89812-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89812-121">Header</span></span>       | <span data-ttu-id="89812-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89812-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89812-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89812-123">Authorization</span></span>  | <span data-ttu-id="89812-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89812-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89812-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89812-126">Content-Type</span></span>  | <span data-ttu-id="89812-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89812-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89812-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89812-129">Request body</span></span>
<span data-ttu-id="89812-130">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89812-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89812-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="89812-131">Response</span></span>

<span data-ttu-id="89812-132">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89812-132">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89812-133">Пример</span><span class="sxs-lookup"><span data-stu-id="89812-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89812-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="89812-134">Request</span></span>
<span data-ttu-id="89812-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89812-135">Here is an example of the request.</span></span>
<span data-ttu-id="89812-136">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89812-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
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

##### <a name="response"></a><span data-ttu-id="89812-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="89812-137">Response</span></span>
<span data-ttu-id="89812-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89812-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
