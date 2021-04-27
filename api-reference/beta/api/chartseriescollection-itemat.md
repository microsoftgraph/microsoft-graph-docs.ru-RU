---
title: 'ChartSeriesCollection: ItemAt'
description: Возвращает ряд на основании сведений о его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ea466f1aeb545f76519b11cc26d0f89bd7e07bc5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047324"
---
# <a name="chartseriescollection-itemat"></a>ChartSeriesCollection: ItemAt

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возвращает ряд на основании сведений о его позиции в коллекции.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|index|number|Значение индекса получаемого объекта. Используется нулевой индекс.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [книгиChartSeries](../resources/workbookchartseries.md) в тексте ответа.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartseriescollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


