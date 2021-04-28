---
title: 'event: delta'
description: 'Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e62229a704ce51b31f0d192107d480ff97f7fd08
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039638"
---
# <a name="event-delta"></a>event: delta

Пространство имен: microsoft.graph

Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.

Вызов функции **delta** для событий схож с отправкой запроса `GET /calendarview` на получение диапазона дат в основном календаре пользователя. С тем исключением, что можно запрашивать добавочные изменения в представлении календаря, правильно применяя [маркеры состояния](/graph/delta-query-overview) при этих вызовах. Это позволяет обслуживать и синхронизировать локальное хранилище таких событий пользователя, не загружая каждый раз все события этого календаря с сервера.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Calendars.Read    |
|Делегированные (личная учетная запись Майкрософт) | Calendars.Read    |
|Для приложений | Calendars.Read |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений в событиях представляет собой цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего отклика в последующих запросах, так как в нем уже содержатся необходимые закодированные параметры.


| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|String|Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".|
|endDateTime|String|Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".|
| $deltatoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для этого же представления календаря и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этого представления календаря.|
| $skiptoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения. |

При выполнении разностного запроса для представления календаря следует ожидать получения всех свойств, которые обычно получают с помощью запроса `GET /calendarview`. `$select` в этом случае не поддерживается. 


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |
| Prefer | string | {Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [event](../resources/event.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество событий в теле отклика двумя.

Чтобы отследить изменения в представлении календаря, выполните один или несколько вызовов функции **delta** с правильными [маркерами состояния](/graph/delta-query-overview), чтобы получить набор добавочных изменений с момента последнего разностного запроса. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
В случае успешного выполнения запроса отклик будет включать маркер состояния — _skipToken_ или _deltaToken_. Первый указан в заголовке отклика _@odata.nextLink_, второй — в заголовке отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.

Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "transactionId": null,
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isDraft": false,
      "isReminderOn": true
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview)
- [Получение добавочных изменений событий в календаре](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

