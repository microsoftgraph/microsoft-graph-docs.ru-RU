---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ce71ac714f2919c1d9c60d71da39a0252b24306c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681657"
---
# <a name="list-calendarview"></a><span data-ttu-id="1637d-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="1637d-103">List calendarView</span></span>

<span data-ttu-id="1637d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1637d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1637d-105">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="1637d-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="1637d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1637d-106">Permissions</span></span>
<span data-ttu-id="1637d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1637d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1637d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1637d-109">Permission type</span></span>      | <span data-ttu-id="1637d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1637d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1637d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1637d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1637d-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1637d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1637d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1637d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1637d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1637d-114">Not supported.</span></span>    |
|<span data-ttu-id="1637d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1637d-115">Application</span></span> | <span data-ttu-id="1637d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1637d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1637d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1637d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="1637d-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1637d-118">Query parameters</span></span>
<span data-ttu-id="1637d-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1637d-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="1637d-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="1637d-120">Parameter</span></span>     | <span data-ttu-id="1637d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1637d-121">Type</span></span>   | <span data-ttu-id="1637d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1637d-122">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1637d-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1637d-123">startDateTime</span></span> | <span data-ttu-id="1637d-124">String</span><span class="sxs-lookup"><span data-stu-id="1637d-124">String</span></span> | <span data-ttu-id="1637d-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1637d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="1637d-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1637d-127">endDateTime</span></span>   | <span data-ttu-id="1637d-128">String</span><span class="sxs-lookup"><span data-stu-id="1637d-128">String</span></span> | <span data-ttu-id="1637d-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1637d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="1637d-131">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и на них не влияет значение заголовка `Prefer: outlook.timezone` при его наличии.</span><span class="sxs-lookup"><span data-stu-id="1637d-131">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="1637d-132">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1637d-132">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="1637d-133">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1637d-133">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1637d-134">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="1637d-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="1637d-135">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="1637d-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1637d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1637d-136">Request headers</span></span>
| <span data-ttu-id="1637d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="1637d-137">Name</span></span>       | <span data-ttu-id="1637d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1637d-138">Type</span></span> | <span data-ttu-id="1637d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1637d-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1637d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="1637d-140">Authorization</span></span>  | <span data-ttu-id="1637d-141">string</span><span class="sxs-lookup"><span data-stu-id="1637d-141">string</span></span> | <span data-ttu-id="1637d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1637d-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1637d-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1637d-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1637d-145">string</span><span class="sxs-lookup"><span data-stu-id="1637d-145">string</span></span> | <span data-ttu-id="1637d-p107">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике. Если он не задан, эти значения времени возвращаются в формате UTC. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="1637d-p107">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |
| <span data-ttu-id="1637d-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1637d-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1637d-150">string</span><span class="sxs-lookup"><span data-stu-id="1637d-150">string</span></span> | <span data-ttu-id="1637d-151">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="1637d-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="1637d-152">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="1637d-152">Values can be "text" or "html".</span></span> <span data-ttu-id="1637d-153">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="1637d-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1637d-154">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="1637d-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="1637d-155">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="1637d-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1637d-156">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1637d-156">Request body</span></span>
<span data-ttu-id="1637d-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1637d-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1637d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="1637d-158">Response</span></span>
<span data-ttu-id="1637d-159">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1637d-159">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1637d-160">Пример</span><span class="sxs-lookup"><span data-stu-id="1637d-160">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1637d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1637d-161">Request</span></span>
<span data-ttu-id="1637d-162">Приведенный ниже пример запрашивает возвращение тел событий в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="1637d-162">The following example requests event bodies to be returned in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="1637d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="1637d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_calendarviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="1637d-164">C#</span><span class="sxs-lookup"><span data-stu-id="1637d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-calendarviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1637d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1637d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-calendarviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1637d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1637d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-calendarviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1637d-167">Java</span><span class="sxs-lookup"><span data-stu-id="1637d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-calendarviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1637d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1637d-168">Response</span></span>
<span data-ttu-id="1637d-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1637d-169">The following is an example of the response.</span></span>
><span data-ttu-id="1637d-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1637d-170">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
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
            "uid":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
            "uid":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
