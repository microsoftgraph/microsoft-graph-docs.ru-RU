---
title: 'event: delta'
description: Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e76bf6cd10682717bebe9365afa14ced47d4c90
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042592"
---
# <a name="event-delta"></a>event: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите набор ресурсов [событий,](../resources/event.md) которые были добавлены, удалены или обновлены в одном или более календарях. 

Вы можете получить определенные типы этих дополнительных изменений в событиях во всех календарях почтового ящика или в определенном календаре или в коллекции событий **calendarView** (диапазон событий, определенных датами начала и окончания) календаря. Календарь может быть календарем по умолчанию или другим указанным календарем пользователя. В случае получения дополнительных изменений **в calendarView** календарь также может быть групповым.

Вызов  функции дельты похож на запрос или запрос указанного календаря, за исключением того, что, надлежащим образом применяя маркеры состояния в одном или несколько из этих вызовов, можно запрашивать дополнительные изменения событий в этом `GET /events` календаре. `GET /calendarview` [](/graph/delta-query-overview#state-tokens) Это позволяет поддерживать и синхронизировать локальный магазин событий в указанном календаре, не извлекая все события календаря с сервера каждый раз.

В следующей таблице перечислены различия между функцией **дельты** событий и функцией дельты в **calendarView** в календаре. 

| Функция Delta в событиях  | Функция Delta в calendarView  |
|:--------------------------|:---------------------------------------------------------|
| Получает дополнительные изменения всех событий в календаре, не ограниченных диапазоном даты начала и окончания. Кроме того, можно получить дополнительные изменения событий в календаре, ограниченных временем начала, начиная с этой даты или после нее. | Получает дополнительные изменения событий в начале и конце **календаря.** |
| Возвращает только ограниченный набор **свойств событий** по соображениям производительности. Клиент для последующего использования `GET /events/{id}` для расширения любых событий. | Расширение на стороне сервера возвращает более полный набор **свойств** событий. |
| Ответ включает в себя отдельные экземпляры и повторяющийся мастер серии. | Ответ включает в себя отдельные экземпляры, а также случаи и исключения повторяющихся серий. |
| Применяется к событиям в календарях пользователей, но не к групповым календарям. | Применяется к событиям в пользовательском и групповом календарях. |
| В настоящее время доступно только в бета-версии. | Доступно в версиях v1.0 и бета-версии. |

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Calendars.Read, Calendars.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Calendars.Read, Calendars.ReadWrite    |
|Для приложений | Calendars.Read, Calendars.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

В этом разделе показан синтаксис  http-запроса для начального вызова функции дельты для запуска полной синхронизации, которая извлекает все события в заданном представлении календаря или календаря. Этот синтаксис не содержит никаких [маркеров состояния.](/graph/delta-query-overview#state-tokens) 

URL-адрес запроса, возвращенный в успешном ответе, включает `nextLink` `deltaLink` маркер состояния. Для любого последующего **вызова функции дельты** используйте URL-адрес запроса в предшествующего `nextLink` или `deltaLink` предшествующего вызова.

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a>Функция Delta в событиях в пользовательском календаре (предварительный просмотр)
Применение **функции дельты** для всех событий или событий, начиная с определенной даты или времени в указанном пользовательском календаре (s):

* Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в почтовом ящике _пользователя:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в календаре по умолчанию _пользователя:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в указанном пользовательском календаре:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в указанной группе календаря и _календаре:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a>Функция Delta в calendarView в пользовательском календаре
Применение **функции дельты** для ряда событий, делимитированные по дате начала и окончания/времени, в указанном пользовательском календаре:

* Чтобы получить дополнительные изменения в представлении календаря календаря пользователя по _умолчанию:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* Чтобы получить дополнительные изменения в представлении календаря указанного _пользовательского календаря:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a>Функция Delta в calendarView в групповом календаре
* Чтобы получить дополнительные изменения в представлении календаря календаря _группы:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений вызывает один или несколько вызовов функции **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе.
В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|String|Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".<br>Часовой пояс указывается в смещенной части часового пояса значения параметра и при этом не влияет на `Prefer: outlook.timezone` заглавный заглавный. Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.<br>Необязательный **для дельты** событий в календаре. <br>Необходимый для **дельты** **в calendarView**. |
|endDateTime|String|Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".<br>Часовой пояс указывается в смещенной части часового пояса значения параметра и при этом не влияет на `Prefer: outlook.timezone` заглавный заглавный. Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.<br>_Не поддерживается_ **дельта** на событиях в календаре. <br>Необходимый для **дельты** **в calendarView**.|
| $deltatoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для этого же представления календаря и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этого представления календаря.|
| $skiptoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения. |

Не поддерживает `$expand` `$filter` , , , и `$orderby` `$select` `$search` .


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |
| Prefer | string | outlook.timezone={Time zone string}. Необязательный, UTC предполагается, если отсутствует.|

## <a name="response"></a>Отклик

### <a name="delta-function-on-events-preview"></a>Функция Delta в событиях (предварительный просмотр)
В случае успешной работы этот метод возвращает код отклика и коллекцию событий `200 OK` в тексте [](../resources/event.md) ответа. **Каждое** событие в ответе содержит только свойства **id,** **type,** **start** и **end** по соображениям производительности. Используйте `GET /events/{id}` впоследствии для расширения любых событий из ответа.  

### <a name="delta-function-on-calendarview"></a>Функция Delta в calendarView
В случае успешной работы этот метод возвращает код отклика и коллекцию событий `200 OK` в тексте [](../resources/event.md) ответа.

Ожидайте получения всех свойств, которые обычно получаются из `GET /calendarview` запроса. 

## <a name="examples"></a>Примеры

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a>Пример 1. Функция Delta для событий в календаре (предварительный просмотр)
#### <a name="request"></a>Запрос
В следующем примере показан начальный запрос на синхронизацию для получения событий в календаре по умолчанию пользователя, которые происходят в указанном параметре или после `startDateTime` него. Начальный запрос не включает какой-либо маркер состояния. 

Запрос использует заглавную для ограничения максимального количества событий в `Prefer: odata.maxpagesize` каждом ответе до 1. Продолжайте вызывать функцию с помощью возвращенного запроса, `delta` `@odata.nextLink` пока не получите `@odata.deltaLink` ответ.

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a>Отклик

Если запрос является успешным, в ответ включается маркер состояния, который является либо _skipToken_ (в загоне ответа _\@ odata.nextLink)_ или _deltaToken_ (в загоне ответа _\@ odata.deltaLink)._
Соответственно, они указывают, следует ли продолжить раунд или вы завершили получение всех изменений для этого раунда.

В ответе ниже показан _skipToken_ в _\@ загоне ответа odata.nextLink._

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a>Пример 2. Функция Delta в calendarView
#### <a name="request"></a>Запрос

В следующем примере показан начальный запрос на синхронизацию для получения событий в заданном календаре подписанного пользователя в диапазоне дат, указанных **в calendarView.** Начальный запрос не включает какой-либо маркер состояния. 

Запрос использует `Prefer: odata.maxpagesize` заглавную для ограничения максимального количества событий в каждом ответе до 2. Продолжайте вызывать функцию с помощью возвращенного запроса, пока не получите все события в этом представлении календаря `delta` `@odata.nextLink` и `@odata.deltaLink` ответ.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Если запрос является успешным, в ответ включается маркер состояния, который является либо _skipToken_ (в загоне ответа _\@ odata.nextLink)_ или _deltaToken_ (в загоне ответа _\@ odata.deltaLink)._
Соответственно, они указывают, следует ли продолжить раунд или вы завершили получение всех изменений для этого раунда.

В ответе ниже показан _skipToken_ в _\@ загоне ответа odata.nextLink._

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](/graph/delta-query-overview)
- [Получение добавочных изменений для событий в папке](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


