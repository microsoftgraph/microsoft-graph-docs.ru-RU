---
title: Создание tableRow
description: Добавьте строки в конец таблицы.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b5299e8db954f1c8e103059115cbb6a7679f2c66
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507563"
---
# <a name="create-tablerow"></a>Создание tableRow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте строки в конец таблицы. 

Обратите внимание, что API может принимать данные нескольких строк с помощью этого API. Добавление одной строки одновременно может привести к снижению производительности. Рекомендуемый подход заключается в том, чтобы совмещение строк в одном вызове, а не вставки одной строки. Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки. Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API. 

Этот запрос может иногда привести к `504 HTTP` ошибке. В этом случае нужно повторить запрос.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbookworksheets/{id|name}/tables/{id|name}/rows
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный.|
| Prefer  | respond-async. Указывает, что запрос является запросом async. Необязательное свойство.  |
| Workbook-Session-Id  | {Workbook-Session-Id}. Создан из **запроса createSession.** Необязательное свойство.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

|Параметр|Тип|Описание|
|:---------------|:--------|:----------|
| index| Int32| Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.|
| values| [Json](../resources/json.md)| Двухмерный массив неформатных значений строк таблицы.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [workbookTableRow](../resources/workbooktablerow.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-two-rows-to-a-table"></a>Пример 1. Добавление двух строк в таблицу

В этом примере в конце таблицы вставляются два ряда данных. 

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json
Content-length: 90

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerowcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```

### <a name="example-2-add-two-rows-to-a-table-asynchronously"></a>Пример 2. Добавление двух строк в таблицу асинхронно

Запросы async будут полезны, если запрос занимает больше времени, чем ожидалось. Обратите внимание, что для выдачи запросов async требуется заглавная `Workbook-Session-Id` заглавная. Перед [использованием](./workbook-createsession.md) функций API с богатым API async пользователю необходимо создать сеанс. Загон `Prefer:respond-async` также требуется в запросах async.

Для функций async пользователю обычно требуется выдавать 2-3 запроса. Этот запрос, [Получить запрос workbookOperation](./workbookoperation-get.md) и необязательный [запрос Get tableRowOperationResult.](./workbook-tablerowoperationresult.md)

#### <a name="request"></a>Запрос

Вот пример запроса async. Обратите внимание, что это произойдет только в том случае, если на ответ `202 Accepted` потребуется много времени. Если запрос будет выполнен быстро, он будет работать как обычный запрос синхронизации, возвращаясь к [примеру 1](#example-1-add-two-rows-to-a-table).


<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json
Prefer: respond-async
Workbook-Session-Id: {Workbook-Session-Id}
Content-length: 51

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```

#### <a name="response"></a>Отклик

Вот еще один пример ответа, который приведет к операции async. Подробные сведения [см. в материале Get workbookOperation](./workbookoperation-get.md) и [Get tableRowOperationResult.](./workbook-tablerowoperationresult.md)
<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "0195cfac-bd22-4f91-b276-dece0aa2378b", "Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ=="],
  "@odata.type": "microsoft.graph.Json"
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/operations/0195cfac-bd22-4f91-b276-dece0aa2378b?sessionId=Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ==
Content-type: application/json
Content-length: 45

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
