---
title: Тип ресурса TableColumn
description: Представляет столбец в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9f70b5363ccc7552975db8f2396af705d8bf1557
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514385"
---
# <a name="tablecolumn-resource-type"></a>Тип ресурса TableColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет столбец в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableColumn](../api/tablecolumn-get.md) | [TableColumn](tablecolumn.md) |Чтение свойств и связей объекта tableColumn.|
|[Обновление](../api/tablecolumn-update.md) | [TableColumn](tablecolumn.md) |Обновление объекта TableColumn. |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[Range](range.md)|Получает объект диапазона, связанный с основными данными столбца.|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой заголовков столбца.|
|[Range](../api/tablecolumn-range.md)|[Range](range.md)|Получает объект диапазона, связанный со всем столбцом.|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой итогов столбца.|
|[Delete](../api/tablecolumn-delete.md)|Нет|Удаляет столбец из таблицы.|
|[Список](../api/tablecolumn-list.md) | Коллекция объектов [TableColumn](tablecolumn.md) |Получение коллекции объектов tableColumn. |
|[Itemat](../api/tablecolumncollection-itemat.md)|[TableColumn](tablecolumn.md)|Возвращает столбец на основании его позиции в коллекции.|
|[Add](../api/tablecolumncollection-add.md)|[TableColumn](tablecolumn.md)|Добавляет новый столбец в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|int|Возвращает уникальный ключ, идентифицирующий столбец в таблице. Только для чтения.|
|index|int|Возвращает номер индекса столбца в коллекции столбцов таблицы. Используется нулевой индекс. Только для чтения.|
|name|строка|Возвращает имя столбца таблицы. Только для чтения.|
|values|json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|filter|[Filter](filter.md)|Возвращает фильтр, применяемый к столбцу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
