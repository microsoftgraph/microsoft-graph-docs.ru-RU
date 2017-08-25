# <a name="user-reminderview"></a><span data-ttu-id="635e4-101">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="635e4-101">user: reminderView</span></span>
<span data-ttu-id="635e4-102">Возвращает список напоминаний календаря за указанный период времени.</span><span class="sxs-lookup"><span data-stu-id="635e4-102">Return a list of calendar reminders within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="635e4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="635e4-103">Permissions</span></span>
<span data-ttu-id="635e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="635e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="635e4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="635e4-106">Permission type</span></span>      | <span data-ttu-id="635e4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="635e4-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="635e4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="635e4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="635e4-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="635e4-109">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="635e4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="635e4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="635e4-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="635e4-111">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="635e4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="635e4-112">Application</span></span> | <span data-ttu-id="635e4-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="635e4-113">Calendars.Read, Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="635e4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="635e4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="635e4-115">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="635e4-115">Function Parameters</span></span>
<span data-ttu-id="635e4-116">В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.</span><span class="sxs-lookup"><span data-stu-id="635e4-116">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="635e4-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="635e4-117">Parameter</span></span>    | <span data-ttu-id="635e4-118">Тип</span><span class="sxs-lookup"><span data-stu-id="635e4-118">Type</span></span>   |<span data-ttu-id="635e4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="635e4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="635e4-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="635e4-120">startDateTime</span></span>|<span data-ttu-id="635e4-121">String</span><span class="sxs-lookup"><span data-stu-id="635e4-121">String</span></span>|<span data-ttu-id="635e4-p102">Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="635e4-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="635e4-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="635e4-124">endDateTime</span></span>|<span data-ttu-id="635e4-125">String</span><span class="sxs-lookup"><span data-stu-id="635e4-125">String</span></span>|<span data-ttu-id="635e4-p103">Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="635e4-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|


## <a name="request-headers"></a><span data-ttu-id="635e4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="635e4-128">Request headers</span></span>
| <span data-ttu-id="635e4-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="635e4-129">Header</span></span>       | <span data-ttu-id="635e4-130">Значение</span><span class="sxs-lookup"><span data-stu-id="635e4-130">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="635e4-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="635e4-131">Authorization</span></span>  | <span data-ttu-id="635e4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="635e4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="635e4-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="635e4-134">Content-Type</span></span>   | <span data-ttu-id="635e4-135">application/json</span><span class="sxs-lookup"><span data-stu-id="635e4-135">application/json</span></span> |
| <span data-ttu-id="635e4-136">Prefer</span><span class="sxs-lookup"><span data-stu-id="635e4-136">Prefer</span></span> | <span data-ttu-id="635e4-p105">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="635e4-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>| 

## <a name="request-body"></a><span data-ttu-id="635e4-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="635e4-139">Request body</span></span>
<span data-ttu-id="635e4-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="635e4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="635e4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="635e4-141">Response</span></span>

<span data-ttu-id="635e4-142">В случае успеха этот метод возвращает код отклика `200, OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="635e4-142">If successful, this method returns `200, OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="635e4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="635e4-143">Example</span></span>
<span data-ttu-id="635e4-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="635e4-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="635e4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="635e4-145">Request</span></span>
<span data-ttu-id="635e4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="635e4-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="635e4-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="635e4-147">Response</span></span>
<span data-ttu-id="635e4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="635e4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
