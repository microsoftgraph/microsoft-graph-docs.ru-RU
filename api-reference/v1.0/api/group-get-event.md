---
title: Вывод события
description: Получение объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ecd831f0f5e0071d0ae0b55d624d11d5f87a887
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720874"
---
# <a name="get-event"></a><span data-ttu-id="bb163-103">Получение события</span><span class="sxs-lookup"><span data-stu-id="bb163-103">Get event</span></span>
<span data-ttu-id="bb163-104">Получение объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="bb163-104">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb163-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb163-105">Permissions</span></span>
<span data-ttu-id="bb163-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb163-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb163-108">Permission type</span></span>      | <span data-ttu-id="bb163-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb163-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb163-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb163-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb163-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb163-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb163-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb163-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb163-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb163-113">Not supported.</span></span>    |
|<span data-ttu-id="bb163-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb163-114">Application</span></span> | <span data-ttu-id="bb163-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb163-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb163-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb163-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb163-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb163-117">Optional query parameters</span></span>
<span data-ttu-id="bb163-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb163-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb163-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb163-119">Request headers</span></span>
| <span data-ttu-id="bb163-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bb163-120">Name</span></span>       | <span data-ttu-id="bb163-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bb163-121">Type</span></span> | <span data-ttu-id="bb163-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bb163-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="bb163-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb163-123">Authorization</span></span>  | <span data-ttu-id="bb163-124">string</span><span class="sxs-lookup"><span data-stu-id="bb163-124">string</span></span> | <span data-ttu-id="bb163-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb163-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb163-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bb163-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="bb163-128">string</span><span class="sxs-lookup"><span data-stu-id="bb163-128">string</span></span> | <span data-ttu-id="bb163-129">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="bb163-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="bb163-130">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bb163-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="bb163-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bb163-131">Optional.</span></span> |
| <span data-ttu-id="bb163-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="bb163-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="bb163-133">string</span><span class="sxs-lookup"><span data-stu-id="bb163-133">string</span></span> | <span data-ttu-id="bb163-134">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="bb163-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="bb163-135">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="bb163-135">Values can be "text" or "html".</span></span> <span data-ttu-id="bb163-136">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="bb163-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="bb163-137">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="bb163-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="bb163-138">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="bb163-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb163-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb163-139">Request body</span></span>
<span data-ttu-id="bb163-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb163-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb163-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb163-141">Response</span></span>
<span data-ttu-id="bb163-142">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bb163-142">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb163-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bb163-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb163-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb163-144">Request</span></span>
<span data-ttu-id="bb163-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb163-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb163-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb163-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "get_group_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb163-147">C#</span><span class="sxs-lookup"><span data-stu-id="bb163-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb163-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb163-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb163-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bb163-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb163-150">Java</span><span class="sxs-lookup"><span data-stu-id="bb163-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb163-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb163-151">Response</span></span>
<span data-ttu-id="bb163-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb163-152">The following is an example of the response.</span></span>
><span data-ttu-id="bb163-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb163-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
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
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
