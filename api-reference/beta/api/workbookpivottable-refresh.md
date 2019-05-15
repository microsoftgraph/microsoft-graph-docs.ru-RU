---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bae547f2397dbc7e19e918c906070fa3177f0d81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961133"
---
# <a name="workbookpivottable-refresh"></a>workbookPivotTable: refresh

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновляет сводную таблицу.


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
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookpivottable_refresh-Javascript-snippets.md)]

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookpivottable_refresh-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-refresh.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookpivottable-refresh.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
