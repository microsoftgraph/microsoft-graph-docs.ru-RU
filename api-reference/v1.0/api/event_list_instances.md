# <a name="list-instances"></a><span data-ttu-id="ac45d-101">Список экземпляров</span><span class="sxs-lookup"><span data-stu-id="ac45d-101">List instances</span></span>

<span data-ttu-id="ac45d-p101">Получение экземпляров события в течение заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события в рамках указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ac45d-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac45d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac45d-104">Prerequisites</span></span>
<span data-ttu-id="ac45d-105">Для применения этого API требуется одна из указанных ниже **областей**. *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="ac45d-105">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="ac45d-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac45d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="ac45d-107">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ac45d-107">Query parameters</span></span>

<span data-ttu-id="ac45d-108">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ac45d-108">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ac45d-109">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac45d-109">Parameter</span></span>    | <span data-ttu-id="ac45d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ac45d-110">Type</span></span>   |<span data-ttu-id="ac45d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ac45d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac45d-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac45d-112">startDateTime</span></span>|<span data-ttu-id="ac45d-113">String</span><span class="sxs-lookup"><span data-stu-id="ac45d-113">String</span></span>|<span data-ttu-id="ac45d-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ac45d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ac45d-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ac45d-116">endDateTime</span></span>|<span data-ttu-id="ac45d-117">String</span><span class="sxs-lookup"><span data-stu-id="ac45d-117">String</span></span>|<span data-ttu-id="ac45d-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ac45d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ac45d-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ac45d-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ac45d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac45d-121">Request headers</span></span>
| <span data-ttu-id="ac45d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ac45d-122">Name</span></span>       | <span data-ttu-id="ac45d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ac45d-123">Type</span></span> | <span data-ttu-id="ac45d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ac45d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ac45d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac45d-125">Authorization</span></span>  | <span data-ttu-id="ac45d-126">string</span><span class="sxs-lookup"><span data-stu-id="ac45d-126">string</span></span>  | <span data-ttu-id="ac45d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac45d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac45d-129">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="ac45d-129">Prefer</span></span> | <span data-ttu-id="ac45d-130">string</span><span class="sxs-lookup"><span data-stu-id="ac45d-130">string</span></span> | <span data-ttu-id="ac45d-p105">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ac45d-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac45d-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac45d-135">Request body</span></span>
<span data-ttu-id="ac45d-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac45d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac45d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac45d-137">Response</span></span>

<span data-ttu-id="ac45d-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac45d-138">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac45d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ac45d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac45d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac45d-140">Request</span></span>
<span data-ttu-id="ac45d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac45d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="ac45d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac45d-142">Response</span></span>
<span data-ttu-id="ac45d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ac45d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
