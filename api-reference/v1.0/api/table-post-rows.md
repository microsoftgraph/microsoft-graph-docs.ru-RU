---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. '
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 546ef8a795683fbd53a850debc1fdc6349538524
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860931"
---
# <a name="create-tablerow"></a>Создание объекта TableRow

Пространство имен: microsoft.graph

Добавляет строки в конец таблицы. 

Обратите внимание, что этот API может принимать несколько строк данных. Добавление одной строки одновременно может повлиять на производительность. Рекомендуемый подход заключается в том, чтобы пакетные строки вместе в одном вызове, а не вставка одной строки. Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки. Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API. 

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
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный.|
| Prefer  | respond-async. Указывает, что запрос является запросом async. Необязательный параметр.  |
| Workbook-Session-Id  | {Workbook-Session-Id}. Создан из **запроса createSession.** Необязательно.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

|Параметр|Тип|Описание|
|:---------------|:--------|:----------|
| index| Int32| Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.|
| values| [Json](../resources/json.md)| Двумерный массив неформатных значений строк таблицы.|

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

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```

### <a name="example-2-add-two-rows-to-a-table-asynchronously"></a>Пример 2. Добавление двух строк в таблицу асинхронно

Запросы async будут полезны, если запрос занимает больше времени, чем ожидалось. Обратите `Workbook-Session-Id` внимание, что загон необходим при выдаче запросов async. Перед [использованием](./workbook-createsession.md) функций API с богатым API async пользователю необходимо создать сеанс. Загон `Prefer:respond-async` также требуется в запросах async.

Для функций async пользователю обычно требуется выдавать два или три запроса: этот запрос, [Get workbookOperation](./workbookoperation-get.md)и необязательный [Get tableRowOperationResult](./workbook-tablerowoperationresult.md).

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
