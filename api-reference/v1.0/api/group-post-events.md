---
title: Создание события
description: Этот API используется для создания события.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 89398b5636734b50c983e5dbb3526b40982d767f
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2019
ms.locfileid: "34310896"
---
# <a name="create-event"></a><span data-ttu-id="a0745-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="a0745-103">Create event</span></span>
<span data-ttu-id="a0745-104">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a0745-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0745-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0745-105">Permissions</span></span>
<span data-ttu-id="a0745-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0745-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0745-108">Permission type</span></span>      | <span data-ttu-id="a0745-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0745-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0745-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0745-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0745-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0745-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0745-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0745-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0745-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0745-113">Not supported.</span></span>    |
|<span data-ttu-id="a0745-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0745-114">Application</span></span> | <span data-ttu-id="a0745-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0745-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0745-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0745-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="a0745-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0745-117">Request headers</span></span>
| <span data-ttu-id="a0745-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0745-118">Header</span></span>       | <span data-ttu-id="a0745-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a0745-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0745-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0745-120">Authorization</span></span>  | <span data-ttu-id="a0745-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0745-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0745-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0745-123">Request body</span></span>
<span data-ttu-id="a0745-124">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0745-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0745-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0745-125">Response</span></span>
<span data-ttu-id="a0745-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0745-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0745-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a0745-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0745-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0745-128">Request</span></span>
<span data-ttu-id="a0745-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0745-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4"],
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2019-06-16T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-06-16T14:00:00",
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
<span data-ttu-id="a0745-130">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0745-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="a0745-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0745-131">Response</span></span>
<span data-ttu-id="a0745-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0745-132">The following is an example of the response.</span></span>
><span data-ttu-id="a0745-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0745-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMK0vA==\"",
    "id": "AAMkADZlEZQbwl7K_XA2LnAAAcwiSBAAA=ZQbwl7K_XA2LnAAAcwiSDAAA=",
    "createdDateTime": "2019-05-20T02:20:45.3057043Z",
    "lastModifiedDateTime": "2019-05-20T02:20:45.5639203Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMK0vA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E008000000005D5775A1B20ED50100000000000000001000000072FA001DBB385A45B6AE65DB0E356105",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does late morning work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZN9uwEZQbwl7K%2BXA2LnAAAAAAENAAA1rwN9uwEZQbwl7K%2BXA2LnAAAcwiSDAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-06-16T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-06-16T14:00:00.0000000",
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
                "address": "adelev@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Retail",
            "address": "Retail@contoso.onmicrosoft.com"
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0745-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a0745-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0745-136">C#</span><span class="sxs-lookup"><span data-stu-id="a0745-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0745-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0745-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
