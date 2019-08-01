---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b5aa7ac82ab997d0e4c9f6a63223be0c1b7892cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014699"
---
# <a name="update-event"></a><span data-ttu-id="78f2c-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="78f2c-103">Update event</span></span>
<span data-ttu-id="78f2c-104">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="78f2c-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="78f2c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78f2c-105">Permissions</span></span>
<span data-ttu-id="78f2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78f2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78f2c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78f2c-108">Permission type</span></span>      | <span data-ttu-id="78f2c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78f2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78f2c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78f2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78f2c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f2c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="78f2c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78f2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f2c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f2c-113">Not supported.</span></span>    |
|<span data-ttu-id="78f2c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78f2c-114">Application</span></span> | <span data-ttu-id="78f2c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78f2c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78f2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="78f2c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78f2c-117">Request headers</span></span>
| <span data-ttu-id="78f2c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="78f2c-118">Name</span></span>       | <span data-ttu-id="78f2c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="78f2c-119">Type</span></span> | <span data-ttu-id="78f2c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="78f2c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="78f2c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f2c-121">Authorization</span></span>  | <span data-ttu-id="78f2c-122">string</span><span class="sxs-lookup"><span data-stu-id="78f2c-122">string</span></span>  | <span data-ttu-id="78f2c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78f2c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78f2c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78f2c-125">Request body</span></span>
<span data-ttu-id="78f2c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="78f2c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="78f2c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="78f2c-129">Response</span></span>
<span data-ttu-id="78f2c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="78f2c-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78f2c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="78f2c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="78f2c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="78f2c-132">Request</span></span>
<span data-ttu-id="78f2c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78f2c-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="78f2c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="78f2c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4", "AAMkADZlAAAAABERAAA="],
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=
Content-type: application/json

{ 
  "location":{
      "displayName":"Conf Room 2"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="78f2c-135">C#</span><span class="sxs-lookup"><span data-stu-id="78f2c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78f2c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="78f2c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78f2c-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="78f2c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="78f2c-138">Java</span><span class="sxs-lookup"><span data-stu-id="78f2c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78f2c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="78f2c-139">Response</span></span>
<span data-ttu-id="78f2c-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="78f2c-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.event",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/calendar/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==\"",
    "id": "AAMkADZlAAAAABERAAA=",
    "createdDateTime": "2019-04-06T13:19:09.2517612Z",
    "lastModifiedDateTime": "2019-05-20T00:14:51.2677891Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B7CA7D517BECD40100000000000000001000000011E38F935AD4FF41BDAB12A2F3E15103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Planogram Training",
    "bodyPreview": "Need more help with visual merchandising?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZlAAAAABERAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Need more help with visual merchandising?\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-04-16T22:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-04-16T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room 2",
        "locationType": "default",
        "uniqueId": "Conf Room 2",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Conf Room 2",
            "locationType": "default",
            "uniqueId": "Conf Room 2",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2019-04-06T13:19:12.1060982Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Retail",
                "address": "Retail@contoso.onmicrosoft.com"
            }
        },
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
                "name": "Nestor Wilke",
                "address": "NestorW@contoso.OnMicrosoft.com"
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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
