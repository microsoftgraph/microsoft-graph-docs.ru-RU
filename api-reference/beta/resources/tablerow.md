---
title: Тип ресурса TableRow
description: Представляет строку в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e1c9dc0f9aad61d815098b76da8620d808c2538a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643750"
---
# <a name="tablerow-resource-type"></a>Тип ресурса TableRow

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableRow](../api/tablerow-get.md) | [TableRow](tablerow.md) |Чтение свойств и связей объекта tableRow.|
|[обновление](../api/tablerow-update.md). | [TableRow](tablerow.md)  |Обновление объекта tableRow. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Возвращает объект диапазона, связанный со всей строкой.|
|[Delete](../api/tablerow-delete.md)|Нет|Удаляет строку из таблицы.|
|[List](../api/tablerow-list.md) | Коллекция объектов [TableRow](tablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|Получает строку на основании сведений о ее позиции в коллекции.|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablerow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
