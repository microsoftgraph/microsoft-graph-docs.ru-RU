# <a name="create-event"></a><span data-ttu-id="d54bd-101">Создание события</span><span class="sxs-lookup"><span data-stu-id="d54bd-101">Create Event</span></span>

<span data-ttu-id="d54bd-102">Создайте [событие](../resources/event.md) в календаре пользователя по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="d54bd-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="d54bd-103">В рамках этих значений вы можете задать часовой пояс для каждого времени начала или окончания события, так как свойства **start** и **end** относятся к типу [dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="d54bd-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="d54bd-104">При отправке события сервер отправляет приглашения всем участникам.</span><span class="sxs-lookup"><span data-stu-id="d54bd-104">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="d54bd-105">**Установка места проведения события**</span><span class="sxs-lookup"><span data-stu-id="d54bd-105">**Setting the location in an event**</span></span>

<span data-ttu-id="d54bd-106">Администратор Exchange может настроить почтовый ящик и адрес электронной почты для ресурса, например конференц-зала, или оборудования, например проектора.</span><span class="sxs-lookup"><span data-stu-id="d54bd-106">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="d54bd-107">Затем пользователи могут пригласить ресурс в качестве участников собрания.</span><span class="sxs-lookup"><span data-stu-id="d54bd-107">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="d54bd-108">Сервер принимает или отклоняет приглашение на собрание от имени ресурса, руководствуясь расписанием его занятости.</span><span class="sxs-lookup"><span data-stu-id="d54bd-108">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="d54bd-109">Если сервер принимает приглашение от имени ресурса, он создает соответствующее событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="d54bd-109">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="d54bd-110">В случае переноса собрания сервер автоматически обновляет событие в календаре ресурса.</span><span class="sxs-lookup"><span data-stu-id="d54bd-110">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="d54bd-111">Еще одно преимущество настройки почтового ящика для ресурса — возможность управления расписанием для ресурса. Например, вы можете разрешить бронирование частного конференц-зала только руководителям и их представителям.</span><span class="sxs-lookup"><span data-stu-id="d54bd-111">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="d54bd-112">Если вы организуете событие, у которого есть место проведения:</span><span class="sxs-lookup"><span data-stu-id="d54bd-112">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="d54bd-113">Задайте соответствующее значение для свойства **location** объекта **event**.</span><span class="sxs-lookup"><span data-stu-id="d54bd-113">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="d54bd-114">Задайте необязательное свойство **locationEmailAddress**, если у места проведения собрания есть адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d54bd-114">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="d54bd-115">Кроме того, если место проведения собрания было настроено как ресурс или для мероприятия требуется какое-либо оборудование, настроенное как ресурс:</span><span class="sxs-lookup"><span data-stu-id="d54bd-115">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="d54bd-116">Пригласите ресурс как объект [attendee](../resources/attendee.md).</span><span class="sxs-lookup"><span data-stu-id="d54bd-116">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="d54bd-117">Задайте для свойства **type** участника значение `resource`.</span><span class="sxs-lookup"><span data-stu-id="d54bd-117">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="d54bd-118">Укажите свойство **emailAddress** участника в качестве электронного адреса ресурса.</span><span class="sxs-lookup"><span data-stu-id="d54bd-118">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="d54bd-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d54bd-119">Permissions</span></span>
<span data-ttu-id="d54bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d54bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d54bd-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d54bd-122">Permission type</span></span>      | <span data-ttu-id="d54bd-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d54bd-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d54bd-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d54bd-124">Delegated (work or school account)</span></span> | <span data-ttu-id="d54bd-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d54bd-125">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d54bd-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d54bd-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d54bd-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d54bd-127">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d54bd-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d54bd-128">Application</span></span> | <span data-ttu-id="d54bd-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d54bd-129">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d54bd-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d54bd-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="d54bd-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d54bd-131">Request headers</span></span>
| <span data-ttu-id="d54bd-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d54bd-132">Header</span></span>       | <span data-ttu-id="d54bd-133">Значение</span><span class="sxs-lookup"><span data-stu-id="d54bd-133">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="d54bd-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d54bd-134">Authorization</span></span>  | <span data-ttu-id="d54bd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d54bd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d54bd-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d54bd-137">Content-Type</span></span>  | <span data-ttu-id="d54bd-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d54bd-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d54bd-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d54bd-140">Request body</span></span>
<span data-ttu-id="d54bd-141">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d54bd-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d54bd-142">Так как ресурс **event** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="d54bd-142">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="d54bd-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="d54bd-143">Response</span></span>

<span data-ttu-id="d54bd-144">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d54bd-144">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d54bd-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d54bd-145">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d54bd-146">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="d54bd-146">Request 1</span></span>
<span data-ttu-id="d54bd-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d54bd-147">Here is an example of the request.</span></span> <span data-ttu-id="d54bd-148">Использует заголовок запроса `Prefer: outlook.timezone`, чтобы указать часовой пояс для параметров времени **start** и **end** в отклике.</span><span class="sxs-lookup"><span data-stu-id="d54bd-148">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>
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
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="d54bd-149">В теле запроса представьте объект [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d54bd-149">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="d54bd-150">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="d54bd-150">Response 1</span></span>
<span data-ttu-id="d54bd-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d54bd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="d54bd-154">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="d54bd-154">Request 2</span></span>
<span data-ttu-id="d54bd-155">Во втором примере показано, как создать повторяющееся событие.</span><span class="sxs-lookup"><span data-stu-id="d54bd-155">The second example shows how to create a recurring event.</span></span> <span data-ttu-id="d54bd-156">Событие происходит с 10:00 до 11:00 каждый понедельник с 4 сентября 2017 г. до конца года.</span><span class="sxs-lookup"><span data-stu-id="d54bd-156">The event occurs from 10:00am to 11:00am, every Monday starting September 4, 2017, through the end of the year.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json

{
  "subject": "Let's go for coffee",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T10:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="d54bd-157">В теле запроса представьте объект [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d54bd-157">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="d54bd-158">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="d54bd-158">Response 2</span></span>
<span data-ttu-id="d54bd-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d54bd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==\"",
    "id":"AAMkADQwMDI5YT",
    "createdDateTime":"2017-10-14T07:37:39.0083072Z",
    "lastModifiedDateTime":"2017-10-14T07:37:40.0239406Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E008000000000068AD4FBF44D301000000000000000010000000CA802EEBDE19CB4AB552714F48C7EEFB",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for coffee",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMDI5YT&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    }
}
```


## <a name="see-also"></a><span data-ttu-id="d54bd-162">См. также</span><span class="sxs-lookup"><span data-stu-id="d54bd-162">See also</span></span>

- [<span data-ttu-id="d54bd-163">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d54bd-163">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d54bd-164">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="d54bd-164">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
