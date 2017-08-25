# <a name="list-instances"></a><span data-ttu-id="ae753-101">Список экземпляров</span><span class="sxs-lookup"><span data-stu-id="ae753-101">List instances</span></span>

<span data-ttu-id="ae753-p101">Получение экземпляров события в течение заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события в рамках указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ae753-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae753-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae753-104">Permissions</span></span>
<span data-ttu-id="ae753-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae753-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae753-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae753-107">Permission type</span></span>      | <span data-ttu-id="ae753-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae753-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ae753-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae753-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ae753-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae753-110">Calendars.Read</span></span>    | 
|<span data-ttu-id="ae753-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae753-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae753-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae753-112">Calendars.Read</span></span>    | 
|<span data-ttu-id="ae753-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae753-113">Application</span></span> | <span data-ttu-id="ae753-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae753-114">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ae753-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae753-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="ae753-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ae753-116">Query parameters</span></span>

<span data-ttu-id="ae753-117">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ae753-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ae753-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae753-118">Parameter</span></span>    | <span data-ttu-id="ae753-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ae753-119">Type</span></span>   |<span data-ttu-id="ae753-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae753-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae753-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ae753-121">startDateTime</span></span>|<span data-ttu-id="ae753-122">String</span><span class="sxs-lookup"><span data-stu-id="ae753-122">String</span></span>|<span data-ttu-id="ae753-p103">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ae753-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ae753-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ae753-125">endDateTime</span></span>|<span data-ttu-id="ae753-126">String</span><span class="sxs-lookup"><span data-stu-id="ae753-126">String</span></span>|<span data-ttu-id="ae753-p104">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ae753-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ae753-129">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ae753-129">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae753-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae753-130">Request headers</span></span>
| <span data-ttu-id="ae753-131">Имя</span><span class="sxs-lookup"><span data-stu-id="ae753-131">Name</span></span>       | <span data-ttu-id="ae753-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ae753-132">Type</span></span> | <span data-ttu-id="ae753-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ae753-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae753-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae753-134">Authorization</span></span>  | <span data-ttu-id="ae753-135">string</span><span class="sxs-lookup"><span data-stu-id="ae753-135">string</span></span>  | <span data-ttu-id="ae753-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae753-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae753-138">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="ae753-138">Prefer</span></span> | <span data-ttu-id="ae753-139">string</span><span class="sxs-lookup"><span data-stu-id="ae753-139">string</span></span> | <span data-ttu-id="ae753-p106">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ae753-p106">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae753-144">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae753-144">Request body</span></span>
<span data-ttu-id="ae753-145">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae753-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae753-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae753-146">Response</span></span>

<span data-ttu-id="ae753-147">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ae753-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae753-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ae753-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae753-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae753-149">Request</span></span>
<span data-ttu-id="ae753-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae753-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="ae753-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae753-151">Response</span></span>
<span data-ttu-id="ae753-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae753-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
