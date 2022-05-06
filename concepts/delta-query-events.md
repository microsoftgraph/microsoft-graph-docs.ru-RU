---
title: 'Получение добавочных изменений для событий в представлении календаря '
description: 'Представление календаря — это коллекция событий в диапазоне дат и времени из календаря по умолчанию (../me/calendarview) '
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 9af9c72f3228dc11ef41884ea9e178494ce0a2ad
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247240"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a>Получение добавочных изменений для событий в представлении календаря 

С помощью разностного запроса можно получить новые, обновленные или удаленные события в указанном календаре(-ях) или в заданном наборе событий (например, в виде представления календаря) в календаре. В этой статье описывается последний случай: получение добавочных изменений для событий в представлении календаря. 

> **Примечание** Возможность получения добавочных изменений для событий календаря, не привязанного к диапазону с фиксированными начальными и конечными датами, относящаяся к первому случаю, в настоящий момент доступна только в бета-версии. Подробнее см. функцию [delta](/graph/api/event-delta).

Представление календаря — это коллекция событий в диапазоне дат и времени (../me/calendarview) из календаря по умолчанию или другого указанного календаря пользователя, или календаря группы. Возвращаемые события могут включать отдельные экземпляры, а также повторения и исключения из повторяющейся серии. Разностные данные позволяют поддерживать и синхронизировать локальное хранилище событий пользователя. При этом вам не требуется каждый раз получать весь набор событий пользователя с сервера.

Запрос изменений поддерживает как полную синхронизацию с получением всех событий в определенном представлении календаря, так и добавочную синхронизацию с получением тех событий, которые изменились в представлении календаря с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения. 

## <a name="track-event-changes-in-a-calendar-view"></a>Отслеживание изменений событий в представлении календаря

Запрос изменений в представлении календаря для событий относится к указанным календарю и диапазону дат и времени. Чтобы отслеживать изменения в нескольких календарях, необходимо наблюдать за каждым календарем отдельно. 

Как правило, цикл отслеживания изменений событий в представлении календаря состоит из одного или нескольких запросов GET с функцией [delta](/graph/api/event-delta). Исходный запрос GET во многом аналогичен [получению списка calendarView](/graph/api/calendar-list-calendarview), но с включением в него функции **delta**. Ниже приведен начальный delta запрос GET представления календаря в календаре по умолчанию вошедшего пользователя.

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

Запрос GET с функцией **delta** возвращает одно из следующих значений:

- ссылку `@odata.nextLink` (содержащую URL-адрес с вызовом функции **delta** и `$skipToken`), или 
- ссылку `@odata.deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `$deltaToken`).

Эти маркеры являются [маркерами состояния](delta-query-overview.md#state-tokens), кодирующими параметры _startDateTime_ и _endDateTime_, а также любой другой параметр в исходном разностном запросе GET. Эти параметры не нужно включать в последующих запросах, поскольку они закодированы в маркерах.

Маркеры состояния полностью непрозрачны для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `@odata.nextLink` или `@odata.deltaLink`, возвращенный последним запросом GET, при следующем вызове функции **delta** для этого представления календаря. Ссылка `@odata.deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `@odata.deltaLink` в начале следующего цикла.

В приведенном ниже [примере](#example-to-synchronize-events-in-a-calendar-view) показано, как использовать URL-адреса `@odata.nextLink` и `@odata.deltaLink`.

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a>Использование параметров запроса изменений для представления календаря

- Укажите параметры _startDateTime_ и _endDateTime_, чтобы определить диапазон дат и времени для представления календаря.
- Параметр `$select` не поддерживается.


### <a name="optional-request-header"></a>Необязательный заголовок запроса

Каждый запрос изменений GET возвращает коллекцию из одного или нескольких событий в ответе. При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество событий в ответе.


## <a name="example-to-synchronize-events-in-a-calendar-view"></a>Пример синхронизации событий в представлении календаря

В приведенном ниже примере показана серия из 3 запросов, синхронизирующих календарь пользователя по умолчанию в определенном диапазоне времени. Это представление календаря содержит 5 событий.

- [Шаг 1. Пример исходного запроса](#step-1-sample-initial-request) и [ответ](#sample-initial-response)
- [Шаг 2. Пример второго запроса](#step-2-sample-second-request) и [ответ](#sample-second-response)
- [Шаг 3. Пример третьего запроса](#step-3-sample-third-request) и [последний ответ](#sample-third-and-final-response)

В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события. 

См. также, что можно сделать в [следующем цикле](#the-next-round-sample-first-response).


### <a name="step-1-sample-initial-request"></a>Шаг 1. Пример исходного запроса

В этом примере указанное представление календаря в календаре по умолчанию пользователя, выполнившего вход, синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле возвращаются все события в представлении календаря.

Первый запрос задает следующие параметры:

- значения даты и времени для параметров _startDateTime_ и _endDateTime_;
- [необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 события одновременно.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a>Пример исходного ответа

Ответ включает два события и заголовок ответа `@odata.nextLink` с маркером `skipToken`. URL-адрес `@odata.nextLink` указывает, что получены не все события в представлении календаря.

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a>Шаг 2. Пример второго запроса

Второй запрос указывает URL-адрес `@odata.nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать те же параметры _startDateTime_ и _endDateTime_, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `@odata.nextLink` кодирует и включает их.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a>Пример второго ответа 

Второй ответ содержит следующие 2 события в представлении календаря и еще одну ссылку `@odata.nextLink`, указывающую, что получены не все события в представлении календаря.

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a>Шаг 3. Пример третьего запроса

Третий запрос продолжает использовать маркер `@odata.nextLink`, полученный из последнего запроса на синхронизацию. 
 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a>Пример третьего и последнего ответа

Третий ответ содержат последнее оставшееся событие из представления календаря и URL-адрес `@odata.deltaLink`, указывающий, что синхронизация для этого представления календаря завершена. Сохраните URL-адрес `@odata.deltaLink` и используйте его в [следующем цикле синхронизации этого представления календаря](#the-next-round-sample-first-request).


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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a>Следующий цикл: пример первого запроса

С помощью ссылки `@odata.deltaLink` из последнего цикла [прошлого запроса](#step-3-sample-third-request) вы сможете получить только те события, которые изменились (путем добавления, удаления или обновления) в этом представлении календаря с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a>Следующий цикл: пример первого ответа

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](delta-query-overview.md)
- [Получение добавочных изменений для сообщений](delta-query-messages.md)
- [Получение добавочных изменений для групп](delta-query-groups.md)
- [Получение добавочных изменений пользователей](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
