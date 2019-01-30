---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640926"
---
# <a name="worksheet-resource-type"></a>Тип ресурса Worksheet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Worksheet](../api/worksheet-get.md) | [Worksheet](worksheet.md) |Чтение свойств и связей объекта листа.|
|[Создание объекта Chart](../api/worksheet-post-charts.md) |[Chart](chart.md)| Создание диаграммы путем добавления в коллекцию диаграмм.|
|[List names](../api/worksheet-list-names.md) |Коллекция объектов [NamedItem](nameditem.md)| Получение коллекции именованных элементов, связанной с листом.|
|[List charts](../api/worksheet-list-charts.md) |Коллекция объектов [Chart](chart.md)| Получение коллекции объектов Chart.|
|[Создание объекта Table](../api/worksheet-post-tables.md) |[Table](table.md)| Создание таблицы путем добавления в коллекцию таблиц.|
|[Список таблиц](../api/worksheet-list-tables.md) |Коллекция объектов [Table](table.md)| Получение коллекции объектов Table.|
|[обновление](../api/worksheet-update.md). | [Worksheet](worksheet.md)   |Обновление объекта Worksheet. |
|[Cell](../api/worksheet-cell.md)|[Range](range.md)|Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.|
|[Range](../api/worksheet-range.md)|[Range](range.md)|Возвращает объект диапазона, указанный по адресу или имени.|
|[Usedrange](../api/worksheet-usedrange.md)|[Range](range.md)|Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.|
|[Delete](../api/worksheet-delete.md)|Нет|Удаляет лист из книги.|
|[List](../api/worksheet-list.md) | Коллекция объектов [Worksheet](worksheet.md) |Получение коллекции объектов листов. |
|[Add](../api/worksheetcollection-add.md)|[Worksheet](worksheet.md)|Добавляет новый лист в книгу. Лист будет добавлен после существующих листов. |
|[Получение списка pivotTables](../api/workbookworksheet-list-pivottables.md) |Коллекция [workbookPivotTable](workbookpivottable.md)| Получение коллекции объектов workbookPivotTable.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.|
|name|строка|Отображаемое имя листа.|
|position|int|Положение листа (начиная с нуля) в книге.|
|visibility|строка|Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|charts|Коллекция объектов [Chart](chart.md)|Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.|
|names|Коллекция объектов [NamedItem](nameditem.md)|Возвращает коллекцию имен, связанных с листом. Только для чтения.|
|pivotTables|Коллекция [workbookPivotTable](workbookpivottable.md)| Коллекция сводных таблиц на листе. |
|protection|[WorksheetProtection](worksheetprotection.md)|Возвращает объект защиты листа. Только для чтения.|
|tables|Коллекция объектов [Table](table.md)|Коллекция таблиц, имеющихся на листе. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
