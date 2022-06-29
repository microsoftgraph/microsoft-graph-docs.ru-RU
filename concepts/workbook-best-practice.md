---
title: Рекомендации по работе с API Excel
description: Советы по работе с API Excel в Microsoft Graph. Узнайте, как управлять сеансами, работать с API, которые занимает много времени, и сократить количество ошибок регулирования.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 6f2b3a0a9c0213098a9a6a214b03e448050a3a1d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447025"
---
# <a name="best-practices-for-working-with-the-excel-api"></a>Рекомендации по работе с API Excel

В этой статье приведены рекомендации по работе с [API Excel](/graph/api/resources/excel) в Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Управление сеансами наиболее эффективным способом

Если у вас есть несколько вызовов в течение определенного периода времени, рекомендуется создать сеанс и передать идентификатор сеанса с каждым запросом. Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`. Таким образом, вы можете использовать API Excel наиболее эффективным способом.

В следующем примере показано, как добавить новое число в таблицу, а затем найти одну запись в книге с помощью этого подхода.

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

Ниже приведен успешный ответ.

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

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Шаг 3. Поиск значения в обновленной таблице

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Шаг 4. Закрытие сеанса после завершения всех запросов

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

Дополнительные сведения см. в разделе ["Создание сеанса](/graph/api/workbook-createsession) " и ["Закрытие сеанса"](/graph/api/workbook-closesession).

## <a name="work-with-apis-that-take-a-long-time-to-complete"></a>Работа с API, выполнение которых занимает много времени

Вы можете заметить, что для выполнения некоторых операций требуется неопределенное время. Например, открытие большой книги. При ожидании ответа на эти запросы можно легко получить время ожидания. Чтобы устранить эту проблему, мы предоставляем шаблон длительных операций. При использовании этого шаблона вам не нужно беспокоиться о времени ожидания запроса.

В настоящее время для API Excel для создания сеансов в Microsoft Graph включена модель длительных операций. Этот шаблон включает в себя следующие действия:

1. Добавьте заголовок `Prefer: respond-async` в запрос, чтобы указать, что это долго выполняемая операция при создании контейнера сеанса.
2. Долго выполняющиеся операции возвращают ответ вместе `202 Accepted` с заголовком Location для получения состояния операции. Если создание сеанса завершится через несколько секунд, он вернет обычный ответ на создание сеанса вместо использования шаблона длительной операции.
3. С помощью `202 Accepted` ответа можно получить состояние операции в указанном расположении. К значениям состояния операции относятся `notStarted`, `running`, и `failed``succeeded`.
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
Шаблон длительных операций вернет ответ `202 Accepted` , аналогичный приведенному ниже.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

В некоторых случаях, если создание завершится успешно в течение нескольких секунд, он не будет вводить шаблон длительных операций; вместо этого он возвращается как обычный сеанс создания, и успешный запрос вернет `201 Created` ответ.

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="poll-status-of-the-long-running-create-session"></a>Состояние опроса продолжительного сеанса создания

С помощью шаблона длительных операций можно получить состояние создания в указанном расположении с помощью следующего запроса. Рекомендуемый интервал опроса составляет около 30 секунд. Максимальный интервал не должен превышать 4 минуты.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Отклик

Ниже приведен ответ, когда операция имеет состояние `running`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

Ниже приведен ответ, когда операция находится в состоянии `succeeded`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

Ниже приведен ответ, когда операция находится в состоянии `failed`.

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

Дополнительные сведения об ошибках см [. в разделе "Коды ошибок и сообщения"](workbook-error-codes.md#error-codes-and-messages).

### <a name="acquire-session-information"></a>Получение сведений о сеансе

#### <a name="request"></a>Запрос

With a status of `succeeded`, you can get the created session information through `resourceLocation` with a request similar to the following.

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

> [!NOTE]
> Получение сведений о сеансе зависит от первоначального запроса. Вам не нужно получать результат, если исходный запрос не возвращает текст ответа.

## <a name="reduce-throttling-errors"></a>Уменьшение количества ошибок регулирования

API Excel в Microsoft Graph влияют на использование ресурсов несколькими службами зависимостей. Влияние может различаться в разных запросах: например, можно ожидать, что обновление короткой строки в одной ячейке небольшой книги будет потреблять меньше ресурсов, чем добавление большой таблицы со сложными формулами в большую книгу.

Даже при работе с тем же API параметры и целевые книги могут привести к значительным различиям. Поэтому регулирование API Excel не определяется простыми и универсальными ограничениями, так как они могут привести к более строгим ограничениям. Приведенные ниже рекомендации помогут быстрее выполнять задачи с помощью меньшего количества ошибок регулирования.

### <a name="retry-after-header"></a>Retry-After заголовка

Во многих случаях ответ регулирования включает заголовок `Retry-After` . Соблюдение значения заголовка и задержка аналогичных запросов поможет клиенту восстановиться после регулирования. Дополнительные сведения об обработке ответов на ошибки из API Excel в Microsoft Graph см. в разделе "Обработка ошибок для [API Excel" в Microsoft Graph](workbook-error-handling.md).

### <a name="throttling-and-concurrency"></a>Регулирование и параллелизм

Еще один фактор, связанный с регулированием, — параллелизм запросов. Не рекомендуется увеличивать параллелизм при использовании API Excel (например, параллелизация запросов к одной книге), особенно для запросов на запись. Вместо этого, если нет определенной проблемы, такой как значительные сетевые издержки по сравнению с очень коротким временем выполнения запроса, рекомендуется последовательное использование в наиболее распространенном случае: для каждой книги отправьте следующий запрос только после получения успешного ответа на текущий запрос.

Параллельные запросы на запись в ту же книгу обычно не выполняются параллельно (хотя в некоторых случаях они выполняются); вместо этого они часто являются причиной регулирования, времени ожидания (когда запросы поставлены в очередь на серверах), конфликта слиянием (при задействовании параллельных сеансов) и других типов сбоев. Они также усложняют обработку ошибок; Например, при ответе на сбой невозможно подтвердить состояние других ожидающих запросов, что затрудняет определение или восстановление состояния книги.

## <a name="see-also"></a>См. также

* [Использование REST API для Excel](/graph/api/resources/excel)