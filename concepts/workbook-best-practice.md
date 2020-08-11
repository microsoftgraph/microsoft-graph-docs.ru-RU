---
title: Рекомендации по использованию API Excel в Microsoft Graph
description: Перечисление рекомендаций и примеров для API Excel в Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ae790dea42e3ade46b74735ad826189a13a282d5
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630349"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>Рекомендации по работе с API Excel в Microsoft Graph

В этой статье приводятся рекомендации по работе с API Excel в Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Наиболее эффективный способ управления сеансами

При наличии нескольких вызовов, которые необходимо выполнить в течение определенного периода времени, рекомендуется создать сеанс и передать ему идентификатор сеанса с каждым запросом. Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`. Таким образом, вы можете использовать API Excel наиболее эффективным способом.

В приведенном ниже примере показано, как добавить в таблицу новый номер, а затем найти одну запись в книге, используя этот подход.

### <a name="step-1-create-a-session"></a>Шаг 1: Создание сеанса

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

Ниже приведен успешный ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>Шаг 2: Добавление новой строки в таблицу

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

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Шаг 3: поиск значения в обновленной таблице

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Шаг 4: закрытие сеанса после завершения всех запросов

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

Более подробную информацию можно узнать в статье [Создание сеанса](/graph/api/workbook-createsession?view=graph-rest-1.0) и [закрытие сеанса](/graph/api/workbook-closesession?view=graph-rest-1.0).

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>Работа с API, для выполнения которых требуется длительное время

Вы можете заметить, что для выполнения некоторых операций требуется неопределенное количество времени; Например, открытие большой книги. При ожидании ответа на эти запросы очень легко достичь времени ожидания ответа. Чтобы устранить эту проблему, мы предоставим долгосрочный шаблон операции. При использовании этого шаблона не нужно беспокоиться об истечении времени ожидания запроса.

В настоящее время в интерфейсе API для создания сеансов в Microsoft Graph включен шаблон длительного выполнения операции. Этот шаблон состоит из следующих этапов:

1. Добавьте `Prefer: respond-async` заголовок в запрос, чтобы указать, что это длительная операция, выполняемая при создании сеанса.
2. При длительной операции возвращается `202 Accepted` ответ вместе с заголовком Location для получения состояния операции. Если создание сеанса завершается через несколько секунд, возвращается обычный ответ на создание сеанса, а не использование долгосрочного шаблона операции.
3. С `202 Accepted` ответом вы можете получить состояние операции в указанном расположении. Значения состояния операции включают `notStarted` , `running` , `succeeded` и `failed` .
4. После завершения операции вы можете получить результат создания сеанса по указанному URL-адресу в ответе, успешном выполнении.

В следующем примере создается сеанс с использованием долгосрочного шаблона операции.

### <a name="initial-request-to-create-session"></a>Первоначальный запрос на создание сеанса

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
Шаблон длительной операции возвращает `202 Accepted` ответ, аналогичный приведенному ниже.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

В некоторых случаях, если создание прошло успешно в течение нескольких секунд, оно не будет вводить шаблон длительной операции; Вместо этого он возвращает как обычный сеанс создания, а успешный запрос возвращает `201 Created` ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

В следующем примере показан ответ при сбое запроса.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json

{
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

### <a name="poll-status-of-the-long-running-create-session"></a>Состояние опроса длительно выполняемого сеанса создания


С помощью шаблона длительной операции вы можете получить состояние создания в указанном расположении с помощью следующего запроса. Рекомендуемый интервал для состояния опроса составляет около 30 секунд. Максимальный интервал не должен превышать 4 минуты.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Отклик

Ниже приведен ответ, в котором находится состояние операции `running` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

Ниже приведен ответ на состояние операции `succeeded` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

Ниже приведен ответ на состояние операции `failed` .

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

Более подробную информацию об ошибках можно узнать в статье [коды ошибок](/concepts/workbook-error-codes.md)

### <a name="acquire-session-information"></a>Получение сведений о сеансе

#### <a name="request"></a>Запрос

С состоянием `succeeded` можно получить сведения о созданном сеансе с помощью `resourceLocation` запроса, аналогичного приведенному ниже.

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

>**Примечание:** Получение сведений о сеансе зависит от первоначального запроса. Нет необходимости приобретать результат, если исходный запрос не возвращает текст отклика.
