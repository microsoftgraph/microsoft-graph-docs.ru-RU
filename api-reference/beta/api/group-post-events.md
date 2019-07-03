---
title: Создание события
description: Этот API используется для создания события.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a9caf57390a0dfa6e6dde82d5351f6c490f70050
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440255"
---
# <a name="create-event"></a><span data-ttu-id="c7efb-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="c7efb-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7efb-104">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c7efb-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7efb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7efb-105">Permissions</span></span>
<span data-ttu-id="c7efb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7efb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7efb-108">Permission type</span></span>      | <span data-ttu-id="c7efb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7efb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7efb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7efb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7efb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7efb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7efb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7efb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7efb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7efb-113">Not supported.</span></span>    |
|<span data-ttu-id="c7efb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7efb-114">Application</span></span> | <span data-ttu-id="c7efb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7efb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7efb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7efb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="c7efb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7efb-117">Request headers</span></span>
| <span data-ttu-id="c7efb-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7efb-118">Header</span></span>       | <span data-ttu-id="c7efb-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c7efb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7efb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7efb-120">Authorization</span></span>  | <span data-ttu-id="c7efb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7efb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7efb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7efb-123">Request body</span></span>
<span data-ttu-id="c7efb-124">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7efb-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7efb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7efb-125">Response</span></span>
<span data-ttu-id="c7efb-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c7efb-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7efb-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c7efb-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c7efb-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7efb-128">Request</span></span>
<span data-ttu-id="c7efb-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7efb-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c7efb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7efb-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4"],
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2019-06-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-06-15T14:00:00",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7efb-131">C#</span><span class="sxs-lookup"><span data-stu-id="c7efb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7efb-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7efb-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7efb-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c7efb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c7efb-134">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7efb-134">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="c7efb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7efb-135">Response</span></span>
<span data-ttu-id="c7efb-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7efb-136">The following is an example of the response.</span></span>
><span data-ttu-id="c7efb-137">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7efb-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7efb-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7efb-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==\"",
    "id": "AAMkADZ_XA2LnAAAcwiSBAAA=",
    "createdDateTime": "2019-05-20T02:14:32.7419058Z",
    "lastModifiedDateTime": "2019-05-20T02:14:33.342409Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000DE7664C3B10ED501000000000000000010000000EC2760BC8BC4AF4BAC1C9730C3E534AC",
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
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZ%2BXA2LnAAAcwiSBAAA%3D&exvsurl=1&path=/calendar/item",
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
        "dateTime": "2019-06-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-06-15T14:00:00.0000000",
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
