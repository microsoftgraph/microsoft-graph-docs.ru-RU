---
title: Создание события
description: Этот API используется для создания события.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d65c77cbe4aab7f6434c6de488eb18a9978d1117
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052266"
---
# <a name="create-event"></a><span data-ttu-id="949dd-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="949dd-103">Create event</span></span>

<span data-ttu-id="949dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="949dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="949dd-105">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="949dd-105">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="949dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="949dd-106">Permissions</span></span>
<span data-ttu-id="949dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="949dd-109">Permission type</span></span>      | <span data-ttu-id="949dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="949dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="949dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="949dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="949dd-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949dd-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="949dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="949dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="949dd-114">Not supported.</span></span>    |
|<span data-ttu-id="949dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="949dd-115">Application</span></span> | <span data-ttu-id="949dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="949dd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="949dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="949dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="949dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="949dd-118">Request headers</span></span>
| <span data-ttu-id="949dd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="949dd-119">Header</span></span>       | <span data-ttu-id="949dd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="949dd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="949dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="949dd-121">Authorization</span></span>  | <span data-ttu-id="949dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="949dd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="949dd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="949dd-124">Request body</span></span>
<span data-ttu-id="949dd-125">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="949dd-125">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="949dd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="949dd-126">Response</span></span>
<span data-ttu-id="949dd-127">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="949dd-127">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949dd-128">Пример</span><span class="sxs-lookup"><span data-stu-id="949dd-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="949dd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="949dd-129">Request</span></span>
<span data-ttu-id="949dd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="949dd-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="949dd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="949dd-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="949dd-132">C#</span><span class="sxs-lookup"><span data-stu-id="949dd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="949dd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="949dd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="949dd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="949dd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="949dd-135">Java</span><span class="sxs-lookup"><span data-stu-id="949dd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="949dd-136">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="949dd-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="949dd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="949dd-137">Response</span></span>
<span data-ttu-id="949dd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="949dd-138">The following is an example of the response.</span></span>
><span data-ttu-id="949dd-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="949dd-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "isDraft": false,
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

