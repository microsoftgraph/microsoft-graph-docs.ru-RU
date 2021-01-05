---
title: Лучшие методики для API Excel в Microsoft Graph
description: Список лучших методик и примеров для API Excel в Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c7e72c4c6480c75d3080d32c2984e6d0f594c409
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754070"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>Best practices for working with the Excel API in Microsoft Graph

В этой статье данная статья содержит рекомендации по работе с API Excel в Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Управление сеансами наиболее эффективным способом

Если в течение определенного периода времени необходимо сделать несколько вызовов, рекомендуется создать сеанс и передать его ИД с каждым запросом. Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`. Таким образом, вы можете использовать API Excel наиболее эффективным способом.

В следующем примере показано, как добавить новый номер в таблицу и найти одну запись в книге с помощью этого подхода.

### <a name="step-1-create-a-session"></a>Шаг 1. Создание сеанса

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a>Отклик

Ниже приводится успешный ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

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
Content-length: 42

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Шаг 3. Найди значение в обновленной таблице

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Шаг 4. Закроем сеанс после завершения всех запросов

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
```

Дополнительные сведения см. в [сведениях о создании сеанса](/graph/api/workbook-createsession?view=graph-rest-1.0) [и закрытии сеанса.](/graph/api/workbook-closesession?view=graph-rest-1.0)

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>Работа с API, которые занять много времени

Вы можете заметить, что для выполнения некоторых операций необходимо определенное время; например, открытие большой книги. При ожидании ответа на эти запросы легко получить время ожидания. Чтобы устранить эту проблему, мы предоставляем долгосрочный шаблон операций. При использовании этого шаблона вам не нужно беспокоиться о времени простоя запроса.

В настоящее время для API Создания сеанса Excel в Microsoft Graph включен долгосрочный шаблон операций. Этот шаблон состоит из следующих этапов:

1. Добавьте в запрос заголок, чтобы указать, что это долго работа при перенастройке `Prefer: respond-async` сеанса.
2. При длительной операции возвращается ответ вместе с заготовом расположением для `202 Accepted` получения состояния операции. Если создание сеанса завершается через несколько секунд, он возвращает обычный ответ на создание сеанса вместо использования длительной операции.
3. С помощью `202 Accepted` отклика можно получить состояние операции в указанном расположении. Значения состояния операции: `notStarted` , , , и `running` `succeeded` `failed` .
4. После завершения операции можно получить результат создания сеанса по указанному URL-адресу в успешном ответе.

В следующем примере создается сеанс с использованием шаблона длительных операций.

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
Шаблон длительных операций возвращает `202 Accepted` ответ, аналогичный следующему.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

В некоторых случаях, если создание успешно в течение нескольких секунд, оно не будет вводить шаблон длительной операции; вместо этого он возвращается в качестве обычного сеанса создания, и успешный запрос возвращает `201 Created` ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

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

### <a name="poll-status-of-the-long-running-create-session"></a>Опрос состояния продолжительного сеанса создания


С помощью шаблона длительной операции можно получить состояние создания в указанном расположении с помощью следующего запроса. Рекомендуемый интервал опроса составляет около 30 секунд. Максимальный интервал не должен быть больше 4 минут.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Отклик

Ниже приводится ответ, когда операция находится в состоянии `running` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

Ниже приводится ответ, когда операция находится в состоянии `succeeded` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

Ниже приводится ответ, когда операция находится в состоянии `failed` .

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

Дополнительные сведения об ошибках см. в [кодах ошибок.](workbook-error-codes.md#error-code)

### <a name="acquire-session-information"></a>Получение сведений о сеансе

#### <a name="request"></a>Запрос

С состоянием ,вы можете получить сведения о созданном сеансе с помощью следующего `succeeded` `resourceLocation` запроса.

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

>**Примечание.** Получение сведений о сеансе зависит от исходного запроса. Вам не нужно получать результат, если исходный запрос не возвращает тело ответа.
