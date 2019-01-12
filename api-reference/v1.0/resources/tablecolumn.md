---
title: Тип ресурса TableColumn
description: Представляет столбец в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15a91ce28509e63f6ca7def284aeafe515ed04d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990833"
---
# <a name="tablecolumn-resource-type"></a>Тип ресурса TableColumn

Представляет столбец в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableColumn](../api/tablecolumn-get.md) | [WorkbookTableColumn](tablecolumn.md) |Чтение свойств и связей объекта tableColumn.|
|[Обновление](../api/tablecolumn-update.md) | [WorkbookTableColumn](tablecolumn.md) |Обновление объекта TableColumn. |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[Range](range.md)|Получает объект диапазона, связанный с основными данными столбца.|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой заголовков столбца.|
|[Range](../api/tablecolumn-range.md)|[Range](range.md)|Получает объект диапазона, связанный со всем столбцом.|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой итогов столбца.|
|[Delete](../api/tablecolumn-delete.md)|Нет|Удаляет столбец из таблицы.|
|[Список](../api/tablecolumn-list.md) | [WorkbookTableColumn](tablecolumn.md) коллекции |Получение коллекции объектов tableColumn. |
|[Itemat](../api/tablecolumncollection-itemat.md)|[WorkbookTableColumn](tablecolumn.md)|Возвращает столбец на основании его позиции в коллекции.|
|[Add](../api/tablecolumncollection-add.md)|[WorkbookTableColumn](tablecolumn.md)|Добавляет новый столбец в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Возвращает уникальный ключ, идентифицирующий столбец в таблице. Это свойство должно интерпретироваться как непрозрачное строковое значение и не должно преобразовываться в любой другой тип. Только для чтения.|
|index|int|Возвращает номер индекса столбца в коллекции столбцов таблицы. Используется нулевой индекс. Только для чтения.|
|name|строка|Возвращает имя столбца таблицы. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|filter|[WorkbookFilter](filter.md)|Возвращает фильтр, применяемый к столбцу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
