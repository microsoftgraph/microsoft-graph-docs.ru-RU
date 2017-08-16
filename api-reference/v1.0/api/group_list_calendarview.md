# <a name="list-calendarview"></a><span data-ttu-id="d02ab-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="d02ab-101">List calendarView</span></span>

<span data-ttu-id="d02ab-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="d02ab-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d02ab-103">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d02ab-103">Prerequisites</span></span>
<span data-ttu-id="d02ab-104">Для применения этого API требуется одна из указанных **областей**: *Group.Read.All* или *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="d02ab-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="d02ab-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d02ab-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="d02ab-106">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d02ab-106">Query parameters</span></span>

<span data-ttu-id="d02ab-107">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d02ab-107">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d02ab-108">Параметр</span><span class="sxs-lookup"><span data-stu-id="d02ab-108">Parameter</span></span>    | <span data-ttu-id="d02ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d02ab-109">Type</span></span>   |<span data-ttu-id="d02ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d02ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d02ab-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d02ab-111">startDateTime</span></span>|<span data-ttu-id="d02ab-112">String</span><span class="sxs-lookup"><span data-stu-id="d02ab-112">String</span></span>|<span data-ttu-id="d02ab-p101">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d02ab-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d02ab-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d02ab-115">endDateTime</span></span>|<span data-ttu-id="d02ab-116">String</span><span class="sxs-lookup"><span data-stu-id="d02ab-116">String</span></span>|<span data-ttu-id="d02ab-p102">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d02ab-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d02ab-119">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d02ab-119">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d02ab-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d02ab-120">Request headers</span></span>
| <span data-ttu-id="d02ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d02ab-121">Header</span></span>       | <span data-ttu-id="d02ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d02ab-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d02ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d02ab-123">Authorization</span></span>  | <span data-ttu-id="d02ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d02ab-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d02ab-126">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="d02ab-126">Prefer</span></span> | <span data-ttu-id="d02ab-127">string</span><span class="sxs-lookup"><span data-stu-id="d02ab-127">string</span></span> | <span data-ttu-id="d02ab-p104">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d02ab-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d02ab-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d02ab-132">Request body</span></span>
<span data-ttu-id="d02ab-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d02ab-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d02ab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02ab-134">Response</span></span>

<span data-ttu-id="d02ab-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d02ab-135">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d02ab-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d02ab-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d02ab-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d02ab-137">Request</span></span>
<span data-ttu-id="d02ab-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d02ab-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="d02ab-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d02ab-139">Response</span></span>
<span data-ttu-id="d02ab-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d02ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
