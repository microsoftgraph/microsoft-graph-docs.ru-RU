---
title: Лучшие практики для Excel API в Microsoft Graph
description: Перечислить лучшие практики и примеры Excel API в Microsoft Graph
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: d5318b51316a20fff00c70df0e655a6058743c29
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944230"
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

В настоящее время создание сеанса Excel API в Microsoft Graph имеет запущенный шаблон работы. Этот шаблон включает в себя следующие действия:

1. Добавьте в запрос заготку, чтобы указать, что при обгонах сеанса операция является `Prefer: respond-async` длительной.
2. При длительной операции возвращается ответ вместе с заготвщиком расположения для `202 Accepted` получения состояния операции. Если создание сеанса завершается за несколько секунд, он возвращает регулярный ответ на создание сеанса вместо использования длительной схемы операции.
3. С помощью `202 Accepted` ответа можно получить состояние операции в указанном расположении. Значения состояния операции включают `notStarted` `running` , и `succeeded` `failed` .
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
Шаблон длительной операции возвращает `202 Accepted` ответ, аналогичный следующему.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

В некоторых случаях, если создание успешно в течение нескольких секунд, оно не будет входить в шаблон длительной операции; вместо этого он возвращается в качестве регулярного сеанса создания, и успешный запрос возвращает `201 Created` ответ.

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

Ниже приводится ответ, когда операция имеет состояние `running` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

Ниже приводится ответ, когда состояние операции `succeeded` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

Ниже приводится ответ, когда состояние операции `failed` .

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

Дополнительные сведения об ошибках см. в [материале "Коды ошибок".](workbook-error-codes.md#error-code)

### <a name="acquire-session-information"></a>Получение сведений о сеансе

#### <a name="request"></a>Запрос

Со статусом , вы можете получить созданную информацию `succeeded` сеанса с `resourceLocation` запросом, похожим на следующие.

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
