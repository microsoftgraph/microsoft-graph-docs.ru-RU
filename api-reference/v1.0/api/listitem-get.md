---
author: JeremyKelley
ms.author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a498947002247541bebf4fc7cd24147a0ca0df7a
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968788"
---
# <a name="get-listitem"></a>Получение ресурса listItem

Возвращает метаданные [элемента][] в [списке][].

[списке]: ../resources/list.md
[элемента]: ../resources/listitem.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Получение ресурса listItem
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
Получение значений столбцов ресурса listItem
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
Получение значений определенных столбцов ресурса listItem
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {код}. Обязательно.|

## <a name="request-body"></a>Основной текст запросов

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик 

При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
