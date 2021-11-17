---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a7374b619fa114c7c1a8f92839e98948988113d2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001014"
---
# <a name="list-events"></a>Перечисление событий

Пространство имен: microsoft.graph

Получение списка событий в календаре.  Это может быть календарь для [пользователя](../resources/user.md) или стандартный календарь для [группы](../resources/group.md) Microsoft 365. В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.

Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).

## <a name="permissions"></a>Разрешения
В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Календарь | Делегированные (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
| календарь пользователя | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite |
| календарь группы | Group.Read.All, Group.ReadWrite.All | Не поддерживается. | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events
```
[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:--------|:--------|
| Authorization  | string | Bearer {токен}. Обязательный.  |
| Prefer: outlook.timezone  | string | С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике. Если он не задан, эти значения времени возвращаются в формате UTC. Необязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="example-1-list-calendar-events"></a>Пример 1. Перечисление событий календаря

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_list_events"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-list-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-list-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-list-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-list-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/calendar-list-events-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик

Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-get-events-by-filtering-on-the-subject-property"></a>Пример 2. Получение событий путем фильтрации по свойству темы

Этот пример получает события из основного календаря пользователя путем фильтрации по их теме, начиная с варианта "Все".

#### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_list_events"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events?$filter=startsWith(subject,'All')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-list-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-list-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-list-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-list-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/calendar-list-events-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('458d4c95-124e-49da-ba9d-1dd0387e682e')/calendar/events",
    "value": [
        {
            "@odata.etag": "W/\"73p1z1T9xUKc8HVNwAwcvgAAR5r+mw==\"",
            "id": "AAMkADBmYTFkMzUyLTgxODQtNDA0YS05YzdlLWRkYjJlY2U4NTljZgBGAAAAAACdCqnIfBTiS7nPzH--j6RvBwDvenXPVP3FQpzwdU3ADBy_AAAAAAENAADvenXPVP3FQpzwdU3ADBy_AABH5Vj3AAA=",
            "createdDateTime": "2021-09-13T13:08:27.8871578Z",
            "lastModifiedDateTime": "2021-09-14T15:14:24.624932Z",
            "changeKey": "73p1z1T9xUKc8HVNwAwcvgAAR5r+mw==",
            "categories": [],
            "transactionId": "f9a93e83-2e8f-a9aa-29af-17b4fe87e221",
            "originalStartTimeZone": "India Standard Time",
            "originalEndTimeZone": "India Standard Time",
            "iCalUId": "040000008200E00074C5B7101A82E008000000001EC43E71A0A8D7010000000000000000100000003FE75E1BE3F09B43BCF2C0EF408DD567",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "All APIs Testing",
            "bodyPreview": "Microsoft Teams meeting",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADBmYTFkMzUyLTgxODQtNDA0YS05YzdlLWRkYjJlY2U4NTljZgBGAAAAAACdCqnIfBTiS7nPzH%2F%2Fj6RvBwDvenXPVP3FQpzwdU3ADBy%2BAAAAAAENAADvenXPVP3FQpzwdU3ADBy%2BAABH5Vj3AAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": true,
            "onlineMeetingProvider": "teamsForBusiness",
            "allowNewTimeProposals": true,
            "isDraft": false,
            "hideAttendees": false,
            "recurrence": null,
            "responseStatus": {
                "response": "organizer",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html><head><meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\"><meta content=\"text/html; charset=us-ascii\"></head><body><br>Microsoft Teams meeting</body></html>"
            },
            "start": {
                "dateTime": "2021-09-14T08:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2021-09-14T08:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "Singapore",
                "locationType": "default",
                "uniqueId": "79e60b5c-bf7e-4811-b314-6eb7f270ec21",
                "uniqueIdType": "locationStore"
            },
            "locations": [
                {
                    "displayName": "Singapore",
                    "locationType": "default",
                    "uniqueId": "79e60b5c-bf7e-4811-b314-6eb7f270ec21",
                    "uniqueIdType": "locationStore"
                }
            ],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "admin@M365B877719.onmicrosoft.com",
                        "address": "admin@M365B877719.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@adatum.onmicrosoft.com"
                }
            },
            "onlineMeeting": {
                "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_YTU5OGEwOTctMjE5NC00ZDQ3LTk5MGMtNWFjNjRmODNhNmVk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22458d4c95-124e-49da-ba9d-1dd0387e682e%22%7d"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
