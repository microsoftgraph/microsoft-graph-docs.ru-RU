---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7c5031a9f2d2729a268f26bb1b1489f3bae2c351
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536493"
---
# <a name="update-an-item-in-a-list"></a>Изменение элемента в списке

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменение свойств ресурса **[listItem][]**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя       | Значение | Описание
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.


## <a name="request-body"></a>Тело запроса

Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.

## <a name="example"></a>Пример

В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.
Все остальные значения для ресурса listItem останутся без изменений. 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```
#### <a name="sdk-sample-code"></a>Образец кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
