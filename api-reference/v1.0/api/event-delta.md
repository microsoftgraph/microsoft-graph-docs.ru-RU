---
title: 'event: delta'
description: 'Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него '
ms.localizationpriority: high
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d25c0c12729a67d991809b3ad5b9f21e514d821
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "62805069"
---
# <a name="event-delta"></a>event: delta

Пространство имен: microsoft.graph

Получение набора ресурсов [event](../resources/event.md), которые были добавлены в **calendarView** (диапазон событий, определяемый датами начала и окончания) основного календаря пользователя, обновлены в нем или удалены из него.

Как правило, синхронизация событий в **calendarView** в локальном хранилище влечет за собой цикл из нескольких вызовов функции **delta**. Исходный вызов связан с полной синхронизацией, а каждый последующий вызов **delta** из того же цикла — с дополнительными изменениями (добавлениями, удалениями или обновлениями). Это позволяет обслуживать и синхронизировать локальное хранилище событий в указанном **calendarView**, не загружая каждый раз все события этого календаря с сервера.

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

### <a name="odata-query-parameters"></a>Параметры запросов OData
- Ожидайте вызова функции **delta** в **calendarView,** чтобы вернуть те же свойства, которые обычно получают с помощью запроса `GET /calendarview`. Вы не можете использовать `$select` для получения только подмножества этих свойств.

- Существуют и другие параметры запросов OData, которые функция **delta** для **calendarView** не поддерживает: `$expand`, `$filter`, `$orderby` и `$search`. 


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |
| Prefer | string | {Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [event](../resources/event.md) в теле отклика.

В цикле вызовов функции **delta**, ограниченном диапазоном дат **calendarView,**, можно найти вызов **delta**, возвращающий два типа событий в `@removed` с причиной `deleted`: 
- События, которые находятся в диапазоне дат и удалены с момента предыдущего вызова **delta**.
- События, которые находятся _за пределами_ диапазона дат и добавлены, удалены или обновлены с момента предыдущего вызова **delta**.

Отфильтруйте события в `@removed` для диапазона дат, которого требует сценарий.

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

