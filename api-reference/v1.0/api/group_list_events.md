# <a name="list-events"></a><span data-ttu-id="fe220-101">Список событий</span><span class="sxs-lookup"><span data-stu-id="fe220-101">List events</span></span>
<span data-ttu-id="fe220-102">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="fe220-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe220-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe220-103">Permissions</span></span>
<span data-ttu-id="fe220-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe220-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe220-106">Permission type</span></span>      | <span data-ttu-id="fe220-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe220-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe220-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe220-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fe220-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe220-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe220-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe220-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe220-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe220-111">Not supported.</span></span>    |
|<span data-ttu-id="fe220-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe220-112">Application</span></span> | <span data-ttu-id="fe220-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe220-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe220-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe220-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe220-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe220-115">Optional query parameters</span></span>
<span data-ttu-id="fe220-116">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe220-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe220-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe220-117">Request headers</span></span>
| <span data-ttu-id="fe220-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe220-118">Header</span></span>       | <span data-ttu-id="fe220-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fe220-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe220-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe220-120">Authorization</span></span>  | <span data-ttu-id="fe220-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe220-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe220-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe220-123">Request body</span></span>
<span data-ttu-id="fe220-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe220-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe220-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe220-125">Response</span></span>
<span data-ttu-id="fe220-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe220-126">If successful, this method returns a `200 OK` response code and a collection of [Event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe220-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fe220-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe220-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe220-128">Request</span></span>
<span data-ttu-id="fe220-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe220-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="fe220-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe220-130">Response</span></span>
<span data-ttu-id="fe220-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe220-131">The following is an example of the response.</span></span>
><span data-ttu-id="fe220-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fe220-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe220-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe220-133">All the properties will be returned from an actual call.</span></span>
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
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
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
