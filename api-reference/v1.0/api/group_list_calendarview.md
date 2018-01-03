# <a name="list-calendarview"></a><span data-ttu-id="487bf-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="487bf-101">List calendarView</span></span>
<span data-ttu-id="487bf-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="487bf-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="487bf-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="487bf-103">Permissions</span></span>
<span data-ttu-id="487bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="487bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="487bf-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="487bf-106">Permission type</span></span>      | <span data-ttu-id="487bf-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="487bf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="487bf-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="487bf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="487bf-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="487bf-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="487bf-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="487bf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="487bf-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="487bf-111">Not supported.</span></span>    |
|<span data-ttu-id="487bf-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="487bf-112">Application</span></span> | <span data-ttu-id="487bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="487bf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="487bf-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="487bf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="487bf-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="487bf-115">Query parameters</span></span>
<span data-ttu-id="487bf-116">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="487bf-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="487bf-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="487bf-117">Parameter</span></span>    | <span data-ttu-id="487bf-118">Тип</span><span class="sxs-lookup"><span data-stu-id="487bf-118">Type</span></span>   |<span data-ttu-id="487bf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="487bf-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="487bf-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="487bf-120">startDateTime</span></span>|<span data-ttu-id="487bf-121">String</span><span class="sxs-lookup"><span data-stu-id="487bf-121">String</span></span>|<span data-ttu-id="487bf-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="487bf-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="487bf-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="487bf-124">endDateTime</span></span>|<span data-ttu-id="487bf-125">String</span><span class="sxs-lookup"><span data-stu-id="487bf-125">String</span></span>|<span data-ttu-id="487bf-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="487bf-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="487bf-128">Этот метод также поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="487bf-128">This method also supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="487bf-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="487bf-129">Request headers</span></span>
| <span data-ttu-id="487bf-130">Имя</span><span class="sxs-lookup"><span data-stu-id="487bf-130">Name</span></span>       | <span data-ttu-id="487bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="487bf-131">Type</span></span> | <span data-ttu-id="487bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="487bf-132">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="487bf-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="487bf-133">Authorization</span></span>  | <span data-ttu-id="487bf-134">string</span><span class="sxs-lookup"><span data-stu-id="487bf-134">string</span></span> | <span data-ttu-id="487bf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="487bf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="487bf-137">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="487bf-137">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="487bf-138">string</span><span class="sxs-lookup"><span data-stu-id="487bf-138">string</span></span> | <span data-ttu-id="487bf-139">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике.</span><span class="sxs-lookup"><span data-stu-id="487bf-139">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="487bf-140">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="487bf-140">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="487bf-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="487bf-141">Optional.</span></span> |
| <span data-ttu-id="487bf-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="487bf-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="487bf-143">string</span><span class="sxs-lookup"><span data-stu-id="487bf-143">string</span></span> | <span data-ttu-id="487bf-144">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="487bf-144">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="487bf-145">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="487bf-145">Values can be "text" or "html".</span></span> <span data-ttu-id="487bf-146">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="487bf-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="487bf-147">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="487bf-147">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="487bf-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="487bf-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="487bf-149">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="487bf-149">Request body</span></span>
<span data-ttu-id="487bf-150">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="487bf-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="487bf-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="487bf-151">Response</span></span>
<span data-ttu-id="487bf-152">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="487bf-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="487bf-153">Пример</span><span class="sxs-lookup"><span data-stu-id="487bf-153">Example</span></span>
#### <a name="request"></a><span data-ttu-id="487bf-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="487bf-154">Request</span></span>
<span data-ttu-id="487bf-155">Приведенный ниже пример запрашивает возвращение тел событий в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="487bf-155">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="487bf-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="487bf-156">Response</span></span>
<span data-ttu-id="487bf-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="487bf-157">The following is an example of the response.</span></span>
><span data-ttu-id="487bf-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="487bf-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="487bf-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="487bf-159">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
