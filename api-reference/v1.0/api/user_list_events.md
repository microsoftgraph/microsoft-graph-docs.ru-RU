# <a name="list-events"></a><span data-ttu-id="e7fee-101">Список событий</span><span class="sxs-lookup"><span data-stu-id="e7fee-101">List events</span></span>

<span data-ttu-id="e7fee-p101">Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="e7fee-104">В настоящее время эта операция возвращает текст события только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="e7fee-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="e7fee-105">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar_list_calendarview.md) или [экземпляры события](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="e7fee-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="e7fee-106">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="e7fee-106">Support various time zones</span></span>

<span data-ttu-id="e7fee-107">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="e7fee-107">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="e7fee-108">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="e7fee-108">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="e7fee-p102">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="e7fee-112">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="e7fee-112">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7fee-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7fee-113">Permissions</span></span>
<span data-ttu-id="e7fee-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7fee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7fee-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7fee-116">Permission type</span></span>      | <span data-ttu-id="e7fee-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7fee-117">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e7fee-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7fee-118">Delegated (work or school account)</span></span> | <span data-ttu-id="e7fee-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fee-119">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="e7fee-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7fee-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7fee-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fee-121">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="e7fee-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7fee-122">Application</span></span> | <span data-ttu-id="e7fee-123">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fee-123">Calendars.Read, Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7fee-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7fee-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7fee-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e7fee-125">Optional query parameters</span></span>
<span data-ttu-id="e7fee-126">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e7fee-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7fee-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7fee-127">Request headers</span></span>
| <span data-ttu-id="e7fee-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e7fee-128">Name</span></span>       | <span data-ttu-id="e7fee-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e7fee-129">Type</span></span> | <span data-ttu-id="e7fee-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e7fee-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e7fee-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7fee-131">Authorization</span></span>  | <span data-ttu-id="e7fee-132">string</span><span class="sxs-lookup"><span data-stu-id="e7fee-132">string</span></span>  | <span data-ttu-id="e7fee-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7fee-135">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e7fee-135">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e7fee-136">string</span><span class="sxs-lookup"><span data-stu-id="e7fee-136">string</span></span> | <span data-ttu-id="e7fee-p105">Часовой пояс по умолчанию для событий, указанных в отклике. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p105">The default time zone for events in the response. Optional.</span></span> | 

## <a name="request-body"></a><span data-ttu-id="e7fee-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7fee-139">Request body</span></span>
<span data-ttu-id="e7fee-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7fee-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7fee-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7fee-141">Response</span></span>

<span data-ttu-id="e7fee-142">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7fee-142">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7fee-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e7fee-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7fee-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7fee-144">Request</span></span>
<span data-ttu-id="e7fee-p106">Ниже приведен пример запроса. Он указывает следующее:</span><span class="sxs-lookup"><span data-stu-id="e7fee-p106">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="e7fee-147">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="e7fee-147">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="e7fee-p107">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p107">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="e7fee-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7fee-150">Response</span></span>
<span data-ttu-id="e7fee-p108">Ниже приведен пример отклика. Свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7fee-p108">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location":{
                "displayName":"Assembly Hall"
            },
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Fanny Downs",
                        "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Fanny Downs",
                    "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
