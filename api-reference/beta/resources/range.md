---
title: Тип ресурса Range
description: Объект Range представляет собой набор из одной или нескольких смежных ячеек, например ячейку, строку, столбец, блок ячеек и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d23b3724dcbcbe7c7bfd26240c5db9eace507b62
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641024"
---
# <a name="range-resource-type"></a>Тип ресурса Range

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект Range представляет собой набор из одной или нескольких смежных ячеек, например ячейку, строку, столбец, блок ячеек и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Range](../api/range-get.md) | [Range](range.md) |Чтение свойств и связей объекта диапазона.|
|[обновление](../api/range-update.md). | [Range](range.md)   |Обновление объекта Range. |
|[Boundingrect](../api/range-boundingrect.md)|[Range](range.md)|Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".|
|[Cell](../api/range-cell.md)|[Range](range.md)|Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.|
|[Column](../api/range-column.md)|[Range](range.md)|Возвращает столбец в диапазоне.|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество столбцов справа от заданного диапазона.|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество столбцов слева от заданного диапазона.|
|[Entirecolumn](../api/range-entirecolumn.md)|[Range](range.md)|Возвращает объект, представляющий весь столбец диапазона.|
|[Entirerow](../api/range-entirerow.md)|[Range](range.md)|Возвращает объект, представляющий всю строку диапазона.|
|[Intersection](../api/range-intersection.md)|[Range](range.md)|Возвращает объект диапазона, представляющий прямоугольное пересечение заданных диапазонов.|
|[Lastcell](../api/range-lastcell.md)|[Range](range.md)|Возвращает последнюю ячейку в диапазоне. Например, последняя ячейка диапазона "B2:D5" — "D5".|
|[Lastcolumn](../api/range-lastcolumn.md)|[Range](range.md)|Возвращает последний столбец в диапазоне. Например, последний столбец диапазона "B2:D5" — "D2:D5".|
|[Lastrow](../api/range-lastrow.md)|[Range](range.md)|Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".|
|[Offsetrange](../api/range-offsetrange.md)|[Range](range.md)|Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.|
|[Row](../api/range-row.md)|[Range](range.md)|Возвращает строку в диапазоне.|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество строк над заданным диапазоном.|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество строк под заданным диапазоном.|
|[Usedrange](../api/range-usedrange.md)|[Range](range.md)|Возвращает используемый диапазон заданного объекта диапазона.|
|[Clear](../api/range-clear.md)|Нет|Очищает значения, формат, заливку, границу диапазона и т. д.|
|[Delete](../api/range-delete.md)|Нет|Удаляет ячейки, связанные с диапазоном.|
|[Insert](../api/range-insert.md)|[Range](range.md)|Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.|
|[Merge](../api/range-merge.md)|Нет|Объединяет ячейки диапазона в одну область на листе.|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.|
|[Unmerge](../api/range-unmerge.md)|Нет|Разъединяет ячейки диапазона на отдельные ячейки.|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|Обеспечивает отображение диапазона в отфильтрованном диапазоне.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|строка|Представляет ссылку на диапазон в стиле A1. Значение адреса будет содержать ссылку на лист (например, Лист1!A1:B4). Только для чтения.|
|addressLocal|строка|Представляет ссылку на указанный диапазон на языке пользователя. Только для чтения.|
|cellCount|int|Количество ячеек в диапазоне. Только для чтения.|
|columnCount|int|Представляет общее количество столбцов в диапазоне. Только для чтения.|
|columnHidden|boolean|Указывает, скрыты ли все столбцы текущего диапазона.|
|columnIndex|int|Представляет номер столбца первой ячейки диапазона. Используется нулевой индекс. Только для чтения.|
|formulas|json|Представляет формулу в формате A1.|
|formulasLocal|json|Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.|
|formulasR1C1|json|Представляет формулу в формате R1C1.|
|hidden|boolean|Указывает, скрыты ли все ячейки текущего диапазона. Только для чтения.|
|numberFormat|json|Представляет код числового формата Excel для данной ячейки.|
|rowCount|int|Возвращает общее количество строк в диапазоне. Только для чтения.|
|rowHidden|boolean|Указывает, скрыты ли все строки текущего диапазона.|
|rowIndex|int|Возвращает номер строки первой ячейки диапазона. Используется нулевой индекс. Только для чтения.|
|text|json|Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.|
|valueTypes|строка|Представляет тип данных каждой ячейки. Возможные значения: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Только для чтения.|
|values|json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[RangeFormat](rangeformat.md)|Возвращает объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона. Только для чтения.|
|sort|[RangeSort](rangesort.md)|Лист, содержащий текущий диапазон. Только для чтения.|
|worksheet|[Worksheet](worksheet.md)|Лист, содержащий текущий диапазон. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.range"
}-->

```json
{
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "json",
  "formulasLocal": "json",
  "formulasR1C1": "json",
  "hidden": true,
  "numberFormat": "json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
