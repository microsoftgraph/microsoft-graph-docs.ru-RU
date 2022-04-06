---
title: Лучшие практики для Excel API в Microsoft Graph
description: Список лучших практик и примеров для Excel API в Microsoft Graph
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 8f1dc872dd94547545c3ca9d47ec08909119e0ea
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672107"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>Наилучшие методы работы с API Excel Microsoft Graph

В этой статье данная статья содержит рекомендации по работе с Excel API в Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Управление сеансами наиболее эффективным способом

Если у вас есть несколько вызовов в течение определенного периода времени, рекомендуем создать сеанс и передать ID сеанса с каждым запросом. Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`. При этом вы можете использовать Excel API наиболее эффективным способом.

В следующем примере показано, как добавить новый номер в таблицу, а затем найти одну запись в книге с помощью этого подхода.

### <a name="step-1-create-a-session"></a>Шаг 1. Создание сеанса

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json

{
  "persistChanges": true
}
```
#### <a name="response"></a>Отклик

Ниже приводится успешный ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>Шаг 2. Добавление новой строки в таблицу

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Шаг 3. Просмотр значения в обновленной таблице

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/functions/vlookup
Content-type: application/json
workbook-session-id: {session-id}

{
    "lookupValue":"pear",
    "tableArray":{"Address":"Sheet1!B2:C7"},
    "colIndexNum":2,
    "rangeLookup":false
}
```

#### <a name="response"></a>Отклик

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Шаг 4. Закрыть сеанс после завершения всех запросов

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}

{
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
```

Дополнительные сведения см. в [материале Create session](/graph/api/workbook-createsession?view=graph-rest-1.0) and [Close session](/graph/api/workbook-closesession?view=graph-rest-1.0).

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>Работа с API, на завершение работы с API уйма времени

Вы можете заметить, что некоторые операции принимают неопределяемую сумму времени для завершения; например, открытие большой книги. В ожидании ответа на эти запросы легко нажать время ожидания. Чтобы устранить эту проблему, мы предоставляем шаблон длительной работы. При использовании этого шаблона не нужно беспокоиться о времени для запроса.

В настоящее время в Excel API Graph Microsoft Graph включена модель длительной работы. Этот шаблон включает в себя следующие действия:

1. Добавьте в `Prefer: respond-async` запрос заготку, чтобы указать, что при обгонах сеанса операция является длительной.
2. При длительной операции возвращается ответ `202 Accepted` вместе с заготвщиком расположения для получения состояния операции. Если создание сеанса завершается за несколько секунд, он возвращает регулярный ответ на создание сеанса вместо использования длительной схемы операции.
3. С помощью `202 Accepted` ответа можно получить состояние операции в указанном расположении. Значения состояния операции включают `notStarted`, `running`и `succeeded``failed`.
4. После завершения операции можно получить результат создания сеанса через указанный URL-адрес в успешном ответе.

В следующем примере создается сеанс с использованием шаблона длительной операции.

### <a name="initial-request-to-create-session"></a>Начальный запрос на создание сеанса

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a>Отклик
Шаблон длительной операции возвращает ответ, `202 Accepted` аналогичный следующему.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

В некоторых случаях, если создание успешно в течение нескольких секунд, оно не будет входить в шаблон длительной операции; вместо этого он возвращается в качестве регулярного сеанса создания, и успешный запрос возвращает ответ `201 Created` .

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

В следующем примере показан ответ при сбойе запроса.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json

{
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": "internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

### <a name="poll-status-of-the-long-running-create-session"></a>Состояние опроса длительной сессии создания


При длительном шаблоне операции можно получить состояние создания в указанном расположении с помощью следующего запроса. Рекомендуемый интервал до состояния опроса составляет около 30 секунд. Максимальный интервал не должен быть более 4 минут.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Отклик

Ниже приводится ответ, когда операция имеет состояние `running`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

Ниже приводится ответ, когда состояние операции `succeeded`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

Ниже приводится ответ, когда состояние операции `failed`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": {operation-id},
  "status": "failed",
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

Дополнительные сведения об ошибках см. в [материале "Коды ошибок"](workbook-error-codes.md#error-code).

### <a name="acquire-session-information"></a>Получение сведений о сеансе

#### <a name="request"></a>Запрос

Со статусом `succeeded`, вы можете получить созданную информацию сеанса с `resourceLocation` запросом, похожим на следующие.

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

#### <a name="response"></a>Отклик
Ниже приведен отклик.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "id-value",
    "persistChanges": true
}
```

>**Примечание:** Получение сведений о сеансе зависит от первоначального запроса. Вам не нужно приобретать результат, если первоначальный запрос не возвращает тело ответа.

## <a name="throttling"></a>Регулирование

Excel API в Microsoft Graph на использование ресурсов нескольких служб зависимостей. Последствия могут различаться между различными запросами: например, можно ожидать, что обновление короткой строки в одной ячейке небольшой книги будет потреблять меньше ресурсов, чем добавление большой таблицы со сложными формулами в большую книгу. Даже при том же API параметры и целевые книги могут привести к значительным различиям. Поэтому Excel регулирования API не определяется простыми и универсальными предельными номерами, так как они могут привести к более строгим ограничениям. Следующие методы помогут быстрее выполнять задачи с помощью меньшего количество ошибок регулирования.

### <a name="retry-after-header"></a>Retry-After

Во многих случаях ответ на регулирование включает в себя загон `Retry-After` . Соблюдение значения загона и задержки аналогичных запросов помогли бы клиенту восстановиться после регулирования. Сведения об обработке ответов на ошибки Excel API в Microsoft Graph см. в Excel [API в Microsoft Graph](workbook-error-handling.md).

### <a name="throttling-and-concurrency"></a>Регулирование и concurrency

Еще один фактор, связанный с регулированием, — это concurrency запроса. Не рекомендуется увеличивать объемы использования Excel API (например, параллелизация запросов с одной и той же книгой), особенно для запросов записи. Вместо этого, если не существует определенной проблемы, например значительных сетевых накладных расходов по сравнению с очень коротким временем выполнения запроса, рекомендуется последовательное использование в наиболее частом случае: для каждой книги отправьте следующий запрос только после получения успешного ответа на текущий запрос.

Параллельные запросы на написание в ту же книгу обычно не запускаются параллельно (хотя в некоторых случаях это происходит); они часто являются причиной регулирования, времени ожидания (когда запросы стоят в очереди на серверах), конфликта слияния (когда участвуют сеансы одновременно) и других типов сбоев. Они также усложняют обработку ошибок; например, когда вы получаете ответ на сбой, невозможно подтвердить состояние других ожидающих запросов, что затрудняет определение или восстановление состояния книги.
