---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7516399af6467a89d6a4e74b88fd0ce127d95141
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720865"
---
# <a name="list-calendarview"></a><span data-ttu-id="a32e0-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="a32e0-103">List calendarView</span></span>
<span data-ttu-id="a32e0-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="a32e0-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a32e0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a32e0-105">Permissions</span></span>
<span data-ttu-id="a32e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a32e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a32e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a32e0-108">Permission type</span></span>      | <span data-ttu-id="a32e0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a32e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a32e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a32e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a32e0-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32e0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a32e0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a32e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a32e0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a32e0-113">Not supported.</span></span>    |
|<span data-ttu-id="a32e0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a32e0-114">Application</span></span> | <span data-ttu-id="a32e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a32e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a32e0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a32e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="a32e0-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="a32e0-117">Query parameters</span></span>
<span data-ttu-id="a32e0-118">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a32e0-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="a32e0-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="a32e0-119">Parameter</span></span>    | <span data-ttu-id="a32e0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a32e0-120">Type</span></span>   |<span data-ttu-id="a32e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a32e0-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32e0-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a32e0-122">startDateTime</span></span>|<span data-ttu-id="a32e0-123">String</span><span class="sxs-lookup"><span data-stu-id="a32e0-123">String</span></span>|<span data-ttu-id="a32e0-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="a32e0-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="a32e0-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a32e0-126">endDateTime</span></span>|<span data-ttu-id="a32e0-127">String</span><span class="sxs-lookup"><span data-stu-id="a32e0-127">String</span></span>|<span data-ttu-id="a32e0-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="a32e0-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="a32e0-130">Этот метод также поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a32e0-130">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="a32e0-131">Свойства **createdDateTime** и **lastModifiedDateTime** для [события](../resources/event.md) не поддерживаются `$select`.</span><span class="sxs-lookup"><span data-stu-id="a32e0-131">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="a32e0-132">Чтобы получить их значения, просто запросите запрос в `$select` **calendarView** , не прибегая к применению.</span><span class="sxs-lookup"><span data-stu-id="a32e0-132">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a32e0-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a32e0-133">Request headers</span></span>
| <span data-ttu-id="a32e0-134">Имя</span><span class="sxs-lookup"><span data-stu-id="a32e0-134">Name</span></span>       | <span data-ttu-id="a32e0-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a32e0-135">Type</span></span> | <span data-ttu-id="a32e0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a32e0-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="a32e0-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a32e0-137">Authorization</span></span>  | <span data-ttu-id="a32e0-138">string</span><span class="sxs-lookup"><span data-stu-id="a32e0-138">string</span></span> | <span data-ttu-id="a32e0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a32e0-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a32e0-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a32e0-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="a32e0-142">string</span><span class="sxs-lookup"><span data-stu-id="a32e0-142">string</span></span> | <span data-ttu-id="a32e0-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="a32e0-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a32e0-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a32e0-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a32e0-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a32e0-145">Optional.</span></span> |
| <span data-ttu-id="a32e0-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a32e0-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a32e0-147">string</span><span class="sxs-lookup"><span data-stu-id="a32e0-147">string</span></span> | <span data-ttu-id="a32e0-148">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="a32e0-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a32e0-149">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="a32e0-149">Values can be "text" or "html".</span></span> <span data-ttu-id="a32e0-150">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="a32e0-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a32e0-151">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="a32e0-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a32e0-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a32e0-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a32e0-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a32e0-153">Request body</span></span>
<span data-ttu-id="a32e0-154">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a32e0-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a32e0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a32e0-155">Response</span></span>
<span data-ttu-id="a32e0-156">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a32e0-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a32e0-157">Пример</span><span class="sxs-lookup"><span data-stu-id="a32e0-157">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a32e0-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a32e0-158">Request</span></span>
<span data-ttu-id="a32e0-159">Приведенный ниже пример запрашивает возвращение тел событий в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="a32e0-159">The following example requests event bodies to be returned in text format.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a32e0-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a32e0-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "group_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a32e0-161">C#</span><span class="sxs-lookup"><span data-stu-id="a32e0-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a32e0-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a32e0-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a32e0-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a32e0-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a32e0-164">Java</span><span class="sxs-lookup"><span data-stu-id="a32e0-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a32e0-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="a32e0-165">Response</span></span>
<span data-ttu-id="a32e0-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a32e0-166">The following is an example of the response.</span></span>
><span data-ttu-id="a32e0-167">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a32e0-167">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a32e0-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a32e0-168">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
