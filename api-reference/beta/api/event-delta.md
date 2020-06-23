---
title: 'event: delta'
description: Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 61ca6937622eadc16aafc1e8c97f38e1fd0db8a2
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845325"
---
# <a name="event-delta"></a>event: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение набора ресурсов [событий](../resources/event.md) , которые были добавлены, удалены или обновлены в одном или нескольких календарях. 

Вы можете получать определенные типы этих добавочных изменений в событиях во всех календарях почтового ящика или в определенном календаре или в коллекции событий **calendarView** (диапазон событий, определенных датами начала и окончания) календаря. Календарь может быть календарем по умолчанию или другим указанным календарем пользователя. Если вы получаете добавочные изменения в **calendarView**, календарь также может быть календарем группы.

Вызов функции **Delta** похож на `GET /events` `GET /calendarview` запрос или запрос для указанного календаря, за исключением того, что при соответствующем применении [маркеров состояния](/graph/delta-query-overview#state-tokens) в одном или нескольких вызовах Вы можете запросить добавочные изменения событий в этой Календер. Это позволяет поддерживать и синхронизировать локальное хранилище событий в указанном календаре без необходимости каждый раз получать все события этого календаря с сервера.

В следующей таблице перечислены различия между функцией **Delta** в событиях и функцией **Delta** в **calendarView** в календаре.

| Функция Delta для событий  | Функция Delta в calendarView  |
|:--------------------------|:---------------------------------------------------------|
| Получает добавочные изменения всех событий в календаре, которые не ограничены диапазоном дат начала и окончания. Кроме того, вы можете получить добавочные изменения событий в календаре, ограниченные временем начала, начиная с или после даты/времени. | Получает добавочные изменения событий в начале и в конце даты и времени **calendarView**. |
| Возвращает ограниченный набор свойств **события** по соображениям производительности. Клиент для последующего использования `GET /events/{id}` для развертывания любых событий. | Расширение на стороне сервера возвращает более полный набор свойств **события** . |
| Ответ включает в себя один экземпляр и образец повторяющегося ряда. | Ответ включает в себя одиночные экземпляры, а также экземпляры и исключения повторяющихся рядов. |
| Применяется к событиям в календарях пользователей, но не календарям групп. | Применяется к событиям в календарях пользователей и групп. |
| В настоящее время доступно только в бета-версии. | Доступно в версиях 1.0 и бета-версиях. |

## <a name="permissions"></a>Разрешения
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Calendars.Read, Calendars.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Calendars.Read, Calendars.ReadWrite    |
|Для приложений | Calendars.Read, Calendars.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

В этом разделе показан синтаксис HTTP-запроса для начального вызова функции **Delta** для запуска полной синхронизации, которая получает все события в указанном календаре или представлении календаря. Этот синтаксис не содержит [маркеров состояния](/graph/delta-query-overview#state-tokens). 

URL-адрес запроса, возвращенный в `nextLink` `deltaLink` ответе или успешном ответе, содержит маркер состояния. Для любого последующего вызова функции **Delta** используйте URL-адрес запроса в `nextLink` `deltaLink` начале или предшествующем ему запросе.

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a>Функция Delta для событий в календаре пользователя (Предварительная версия)
Примените функцию **Delta** ко всем событиям или событиям, начиная с определенной даты/времени или после нее, в указанных календарях пользователей:

* Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в почтовом ящике пользователя_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* Для получения добавочных изменений всех событий или событий, начиная с указанной даты или после указанной даты и времени _в календаре пользователя по умолчанию_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанном календаре пользователя_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанном календаре группы календарей по умолчанию_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroup/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta 

  GET /me/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанной группе календаря и календаре_:
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

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a>Функция Delta в calendarView в календаре пользователя
Примените функцию **Delta** к диапазону событий, разделенных на дату начала и окончания, в указанном календаре пользователя:

* Для получения добавочных изменений в представлении календаря _календаря пользователя по умолчанию_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* Чтобы получить добавочные изменения в представлении календаря для _указанного календаря пользователя_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a>Функция Delta в calendarView в календаре группы
* Чтобы получить добавочные изменения в представлении календаря _группы_, выполните следующие действия:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе.
При последующих запросах просто скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа, так как этот URL-адрес уже включает закодированные, нужные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|String|The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00". <br>Часовой пояс указывается в части смещения TimeZone значения параметра и не влияет на `Prefer: outlook.timezone` заголовку, если он есть. Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.<br>Необязательно для **изменений** событий в календаре. <br>Обязательный для **изменений** в **calendarView**. |
|endDateTime|String|The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00". <br>Часовой пояс указывается в части смещения TimeZone значения параметра и не влияет на `Prefer: outlook.timezone` заголовку, если он есть. Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.<br>_Не поддерживается_ в **Delta** для событий в календаре. <br>Обязательный для **изменений** в **calendarView**.|
| $deltatoken | string | A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.|
| $skiptoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения. |

Не поддерживает `$expand` , `$filter` ,, `$orderby` `$select` и `$search` .


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Required. |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}. Optional. |
| Prefer | string | Outlook. TimeZone = {строка часового пояса}. Необязательное, в формате UTC предполагается, что отсутствует.|

## <a name="response"></a>Отклик

### <a name="delta-function-on-events-preview"></a>Функция Delta для событий (Предварительная версия)
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [событий](../resources/event.md) в тексте отклика. Каждое **событие** в ответе содержит только свойства **ID**, **Type**, **Start** и **End** для повышения производительности. Используйте `GET /events/{id}` последовательное, чтобы развернуть все события из отклика.  

### <a name="delta-function-on-calendarview"></a>Функция Delta в calendarView
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [событий](../resources/event.md) в тексте отклика.

Ожидается получение всех свойств, которые вы обычно получаете из `GET /calendarview` запроса. 

## <a name="examples"></a>Примеры

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a>Пример 1: функция Delta для событий в календаре (Предварительная версия)
#### <a name="request"></a>Запрос
В следующем примере показан первоначальный запрос на синхронизацию для получения событий в календаре пользователя, вошедшего в систему по умолчанию, которые происходят в указанном параметре или после него `startDateTime` . Исходный запрос не включает никаких маркеров состояния. 

В запросе используется `Prefer: odata.maxpagesize` заголовок, чтобы ограничить максимальное количество событий в каждом ответе на 1. Продолжайте вызывать `delta` функцию с помощью запроса, возвращенного в `@odata.nextLink` `@odata.deltaLink` ответе.

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a>Отклик

Если запрос выполнен успешно, ответ включает маркер состояния, который является либо _skipToken_ (в заголовке ответа _ \@ OData. NextLink_ ), либо _deltaToken_ (в заголовке ответа _ \@ OData. deltaLink_ ).
В соответствии с этим они указывают, следует ли продолжать работу со циклом или вы завершили сбор всех изменений для этого цикла.

Приведенный ниже ответ показывает _skipToken_ в заголовке ответа _ \@ OData. nextLink_ .

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


### <a name="example-2-delta-function-on-calendarview"></a>Пример 2: функция Delta в calendarView
#### <a name="request"></a>Запрос

В приведенном ниже примере показан первоначальный запрос на синхронизацию для получения событий в указанном календаре вошедшего пользователя, в диапазоне дат, указанном с помощью **calendarView**. Исходный запрос не включает никаких маркеров состояния. 

В запросе используется `Prefer: odata.maxpagesize` заголовок, чтобы ограничить максимальное количество событий в каждом ответе на 2. Продолжите вызов `delta` функции с помощью запроса, возвращенного, `@odata.nextLink` пока не будут получены все события в представлении календаря и `@odata.deltaLink` в ответе.

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
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Если запрос выполнен успешно, ответ включает маркер состояния, который является либо _skipToken_ (в заголовке ответа _ \@ OData. NextLink_ ), либо _deltaToken_ (в заголовке ответа _ \@ OData. deltaLink_ ).
В соответствии с этим они указывают, следует ли продолжать работу со циклом или вы завершили сбор всех изменений для этого цикла.

Приведенный ниже ответ показывает _skipToken_ в заголовке ответа _ \@ OData. nextLink_ .

Примечание. Представленный здесь объект отклика может быть усечен для краткости. 
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

### <a name="see-also"></a>См. также

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
