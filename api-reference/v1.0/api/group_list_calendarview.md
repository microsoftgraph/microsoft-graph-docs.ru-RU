# <a name="list-calendarview"></a><span data-ttu-id="ba5be-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="ba5be-101">List calendarView</span></span>
<span data-ttu-id="ba5be-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря группы, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="ba5be-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba5be-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5be-103">Permissions</span></span>
<span data-ttu-id="ba5be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba5be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba5be-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5be-106">Permission type</span></span>      | <span data-ttu-id="ba5be-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba5be-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba5be-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba5be-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ba5be-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5be-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba5be-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba5be-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba5be-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba5be-111">Not supported.</span></span>    |
|<span data-ttu-id="ba5be-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba5be-112">Application</span></span> | <span data-ttu-id="ba5be-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba5be-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba5be-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba5be-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="ba5be-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ba5be-115">Query parameters</span></span>
<span data-ttu-id="ba5be-116">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ba5be-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ba5be-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="ba5be-117">Parameter</span></span>    | <span data-ttu-id="ba5be-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5be-118">Type</span></span>   |<span data-ttu-id="ba5be-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5be-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba5be-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5be-120">startDateTime</span></span>|<span data-ttu-id="ba5be-121">String</span><span class="sxs-lookup"><span data-stu-id="ba5be-121">String</span></span>|<span data-ttu-id="ba5be-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ba5be-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ba5be-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5be-124">endDateTime</span></span>|<span data-ttu-id="ba5be-125">String</span><span class="sxs-lookup"><span data-stu-id="ba5be-125">String</span></span>|<span data-ttu-id="ba5be-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ba5be-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ba5be-128">Этот метод также поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba5be-128">This method also supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba5be-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba5be-129">Request headers</span></span>
| <span data-ttu-id="ba5be-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba5be-130">Header</span></span>       | <span data-ttu-id="ba5be-131">Значение</span><span class="sxs-lookup"><span data-stu-id="ba5be-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba5be-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba5be-132">Authorization</span></span>  | <span data-ttu-id="ba5be-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba5be-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba5be-135">Prefer</span><span class="sxs-lookup"><span data-stu-id="ba5be-135">Prefer</span></span> | <span data-ttu-id="ba5be-136">string</span><span class="sxs-lookup"><span data-stu-id="ba5be-136">string</span></span> | <span data-ttu-id="ba5be-p105">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ba5be-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba5be-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba5be-141">Request body</span></span>
<span data-ttu-id="ba5be-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba5be-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba5be-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba5be-143">Response</span></span>
<span data-ttu-id="ba5be-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba5be-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5be-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ba5be-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ba5be-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba5be-146">Request</span></span>
<span data-ttu-id="ba5be-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba5be-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```

#### <a name="response"></a><span data-ttu-id="ba5be-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba5be-148">Response</span></span>
<span data-ttu-id="ba5be-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba5be-149">The following is an example of the response.</span></span>
><span data-ttu-id="ba5be-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba5be-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba5be-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba5be-151">All the properties will be returned from an actual call.</span></span>
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
