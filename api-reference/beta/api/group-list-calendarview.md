---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.
ms.openlocfilehash: 25090591750ed556407159f3744113b08d25fcae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077854"
---
# <a name="list-calendarview"></a><span data-ttu-id="8ec4c-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="8ec4c-103">List calendarView</span></span>

> <span data-ttu-id="8ec4c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ec4c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ec4c-106">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ec4c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec4c-107">Permissions</span></span>
<span data-ttu-id="8ec4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec4c-110">Permission type</span></span>      | <span data-ttu-id="8ec4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ec4c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ec4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ec4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ec4c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec4c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ec4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ec4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-115">Not supported.</span></span>    |
|<span data-ttu-id="8ec4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ec4c-116">Application</span></span> | <span data-ttu-id="8ec4c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ec4c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ec4c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="8ec4c-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8ec4c-119">Query parameters</span></span>
<span data-ttu-id="8ec4c-120">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="8ec4c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ec4c-121">Parameter</span></span>    | <span data-ttu-id="8ec4c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8ec4c-122">Type</span></span>   |<span data-ttu-id="8ec4c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec4c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ec4c-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec4c-124">startDateTime</span></span>|<span data-ttu-id="8ec4c-125">String</span><span class="sxs-lookup"><span data-stu-id="8ec4c-125">String</span></span>|<span data-ttu-id="8ec4c-p103">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="8ec4c-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="8ec4c-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec4c-128">endDateTime</span></span>|<span data-ttu-id="8ec4c-129">String</span><span class="sxs-lookup"><span data-stu-id="8ec4c-129">String</span></span>|<span data-ttu-id="8ec4c-p104">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="8ec4c-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="8ec4c-132">Этот метод также поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-132">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ec4c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ec4c-133">Request headers</span></span>
| <span data-ttu-id="8ec4c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="8ec4c-134">Name</span></span>       | <span data-ttu-id="8ec4c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8ec4c-135">Type</span></span> | <span data-ttu-id="8ec4c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec4c-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8ec4c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ec4c-137">Authorization</span></span>  | <span data-ttu-id="8ec4c-138">string</span><span class="sxs-lookup"><span data-stu-id="8ec4c-138">string</span></span> | <span data-ttu-id="8ec4c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ec4c-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8ec4c-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8ec4c-142">string</span><span class="sxs-lookup"><span data-stu-id="8ec4c-142">string</span></span> | <span data-ttu-id="8ec4c-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8ec4c-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8ec4c-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-145">Optional.</span></span> |
| <span data-ttu-id="8ec4c-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8ec4c-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8ec4c-147">string</span><span class="sxs-lookup"><span data-stu-id="8ec4c-147">string</span></span> | <span data-ttu-id="8ec4c-148">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="8ec4c-149">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="8ec4c-149">Values can be "text" or "html".</span></span> <span data-ttu-id="8ec4c-150">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="8ec4c-151">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="8ec4c-152">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ec4c-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ec4c-153">Request body</span></span>
<span data-ttu-id="8ec4c-154">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ec4c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec4c-155">Response</span></span>
<span data-ttu-id="8ec4c-156">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec4c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8ec4c-157">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8ec4c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ec4c-158">Request</span></span>
<span data-ttu-id="8ec4c-159">Приведенный ниже пример запрашивает возвращение тел событий в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-159">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarviews"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="8ec4c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec4c-160">Response</span></span>
<span data-ttu-id="8ec4c-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-161">The following is an example of the response.</span></span>
><span data-ttu-id="8ec4c-162">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8ec4c-163">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ec4c-163">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
