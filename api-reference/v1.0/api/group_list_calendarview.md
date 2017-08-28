# <a name="list-calendarview"></a><span data-ttu-id="98aa3-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="98aa3-101">List calendarView</span></span>

<span data-ttu-id="98aa3-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="98aa3-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="permissions"></a><span data-ttu-id="98aa3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98aa3-103">Permissions</span></span>
<span data-ttu-id="98aa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98aa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98aa3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98aa3-106">Permission type</span></span>      | <span data-ttu-id="98aa3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98aa3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98aa3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98aa3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="98aa3-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98aa3-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98aa3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98aa3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98aa3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98aa3-111">Not supported.</span></span>    |
|<span data-ttu-id="98aa3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98aa3-112">Application</span></span> | <span data-ttu-id="98aa3-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98aa3-113">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98aa3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98aa3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="98aa3-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="98aa3-115">Query parameters</span></span>

<span data-ttu-id="98aa3-116">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="98aa3-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="98aa3-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="98aa3-117">Parameter</span></span>    | <span data-ttu-id="98aa3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="98aa3-118">Type</span></span>   |<span data-ttu-id="98aa3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="98aa3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98aa3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98aa3-120">startDateTime</span></span>|<span data-ttu-id="98aa3-121">String</span><span class="sxs-lookup"><span data-stu-id="98aa3-121">String</span></span>|<span data-ttu-id="98aa3-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="98aa3-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="98aa3-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="98aa3-124">endDateTime</span></span>|<span data-ttu-id="98aa3-125">String</span><span class="sxs-lookup"><span data-stu-id="98aa3-125">String</span></span>|<span data-ttu-id="98aa3-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="98aa3-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="98aa3-128">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="98aa3-128">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="98aa3-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98aa3-129">Request headers</span></span>
| <span data-ttu-id="98aa3-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98aa3-130">Header</span></span>       | <span data-ttu-id="98aa3-131">Значение</span><span class="sxs-lookup"><span data-stu-id="98aa3-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98aa3-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98aa3-132">Authorization</span></span>  | <span data-ttu-id="98aa3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98aa3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98aa3-135">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="98aa3-135">Prefer</span></span> | <span data-ttu-id="98aa3-136">string</span><span class="sxs-lookup"><span data-stu-id="98aa3-136">string</span></span> | <span data-ttu-id="98aa3-p105">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="98aa3-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98aa3-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98aa3-141">Request body</span></span>
<span data-ttu-id="98aa3-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98aa3-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98aa3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="98aa3-143">Response</span></span>

<span data-ttu-id="98aa3-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="98aa3-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98aa3-145">Пример</span><span class="sxs-lookup"><span data-stu-id="98aa3-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98aa3-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="98aa3-146">Request</span></span>
<span data-ttu-id="98aa3-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98aa3-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="98aa3-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="98aa3-148">Response</span></span>
<span data-ttu-id="98aa3-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="98aa3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
