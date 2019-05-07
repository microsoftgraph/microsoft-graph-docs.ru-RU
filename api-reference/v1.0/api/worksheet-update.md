---
title: Обновление листа
description: Обновление свойств объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5287148ab57eb6d0c3a39184248f673391dafd44
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600541"
---
# <a name="update-worksheet"></a>Обновление листа

Обновление свойств объекта листа.
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
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Отображаемое имя листа.|
|position|int|Положение листа (начиная с нуля) в книге.|
|visibility|string|Видимость листа. Допустимые значения: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукворкшит](../resources/worksheet.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/update_worksheet-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_worksheet-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
