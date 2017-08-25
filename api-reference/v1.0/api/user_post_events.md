# <a name="create-event"></a><span data-ttu-id="2439f-101">Создание события</span><span class="sxs-lookup"><span data-stu-id="2439f-101">Create Event</span></span>

<span data-ttu-id="2439f-102">Создайте [событие](../resources/event.md) в календаре пользователя по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="2439f-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="2439f-103">В рамках этих значений вы можете задать часовой пояс для каждого времени начала или окончания события, так как свойства **start** и **end** относятся к типу [dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="2439f-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="2439f-104">При создании события сервер отправляет приглашения всем участникам.</span><span class="sxs-lookup"><span data-stu-id="2439f-104">When the event is created, the server send invitations to all attendees.</span></span>


## <a name="permissions"></a><span data-ttu-id="2439f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2439f-105">Permissions</span></span>
<span data-ttu-id="2439f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2439f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2439f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2439f-108">Permission type</span></span>      | <span data-ttu-id="2439f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2439f-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2439f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2439f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2439f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2439f-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2439f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2439f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2439f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2439f-113">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2439f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2439f-114">Application</span></span> | <span data-ttu-id="2439f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2439f-115">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2439f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2439f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="2439f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2439f-117">Request headers</span></span>
| <span data-ttu-id="2439f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2439f-118">Header</span></span>       | <span data-ttu-id="2439f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="2439f-119">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="2439f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2439f-120">Authorization</span></span>  | <span data-ttu-id="2439f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2439f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2439f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2439f-123">Content-Type</span></span>  | <span data-ttu-id="2439f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2439f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2439f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2439f-126">Request body</span></span>
<span data-ttu-id="2439f-127">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2439f-127">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="2439f-128">Так как ресурс **event** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="2439f-128">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="2439f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2439f-129">Response</span></span>

<span data-ttu-id="2439f-130">В случае успеха этот метод возвращает код ответа `201, Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2439f-130">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2439f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2439f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2439f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2439f-132">Request</span></span>
<span data-ttu-id="2439f-p104">Ниже приведен пример запроса. В нем используется заголовок запроса `Prefer: outlook.timezone`, чтобы указать, что для параметров времени **start** и **end** в ответе следует использовать этот часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="2439f-p104">Here is an example of the request. It uses the `Prefer: outlook.timezone` request header to specify the **start** and **end** times in the response should use that time zone.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"fannyd@contoso.onmicrosoft.com",
        "name": "Fanny Downs"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="2439f-135">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2439f-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2439f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2439f-136">Response</span></span>
<span data-ttu-id="2439f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2439f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
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
                "name":"Fanny Downs",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```
## <a name="see-also"></a><span data-ttu-id="2439f-140">См. также</span><span class="sxs-lookup"><span data-stu-id="2439f-140">See also</span></span>

- [<span data-ttu-id="2439f-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2439f-141">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2439f-142">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2439f-142">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
