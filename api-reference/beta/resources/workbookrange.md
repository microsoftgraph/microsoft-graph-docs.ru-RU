---
title: Тип ресурса workbookRange
description: Объект Range представляет собой набор из одной или нескольких смежных ячеек, например ячейку, строку, столбец, блок ячеек и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 23748b2f92d8ba786ba6e8ef82df0243f9fe2617
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519199"
---
# <a name="workbookrange-resource-type"></a>Тип ресурса workbookRange

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект Range представляет собой набор из одной или нескольких смежных ячеек, например ячейку, строку, столбец, блок ячеек и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Range](../api/range-get.md) | [workbookRange](workbookrange.md) |Чтение свойств и связей объекта диапазона.|
|[Обновление](../api/range-update.md) | [workbookRange](workbookrange.md)   |Обновление объекта Range. |
|[Boundingrect](../api/range-boundingrect.md)|[workbookRange](workbookrange.md)|Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".|
|[Cell](../api/range-cell.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.|
|[Column](../api/range-column.md)|[workbookRange](workbookrange.md)|Возвращает столбец в диапазоне.|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество столбцов справа от заданного диапазона.|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество столбцов слева от заданного диапазона.|
|[Entirecolumn](../api/range-entirecolumn.md)|[workbookRange](workbookrange.md)|Возвращает объект, представляющий весь столбец диапазона.|
|[Entirerow](../api/range-entirerow.md)|[workbookRange](workbookrange.md)|Возвращает объект, представляющий всю строку диапазона.|
|[Intersection](../api/range-intersection.md)|[workbookRange](workbookrange.md)|Возвращает объект диапазона, представляющий прямоугольное пересечение заданных диапазонов.|
|[Lastcell](../api/range-lastcell.md)|[Range](workbookrange.md)|Возвращает последнюю ячейку в диапазоне. Например, последняя ячейка диапазона B2:D5 — D5.|
|[Lastcolumn](../api/range-lastcolumn.md)|[workbookRange](workbookrange.md)|Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.|
|[Lastrow](../api/range-lastrow.md)|[Range](workbookrange.md)|Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".|
|[Offsetrange](../api/range-offsetrange.md)|[workbookRange](workbookrange.md)|Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.|
|[Row](../api/range-row.md)|[Range](workbookrange.md)|Возвращает строку из диапазона.|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество строк над заданным диапазоном.|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Возвращает определенное количество строк под заданным диапазоном.|
|[Usedrange](../api/range-usedrange.md)|[workbookRange](workbookrange.md)|Возвращает используемый диапазон заданного объекта диапазона.|
|[Clear](../api/range-clear.md)|Нет|Очищает значения, формат, заливку, границу диапазона и т. д.|
|[Delete](../api/range-delete.md)|Нет.|Удаляет ячейки, связанные с диапазоном.|
|[Insert](../api/range-insert.md)|[workbookRange](workbookrange.md)|Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.|
|[Merge](../api/range-merge.md)|Нет|Объединяет ячейки диапазона в одну область на листе.|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.|
|[Unmerge](../api/range-unmerge.md)|Нет|Разъединяет ячейки диапазона на отдельные ячейки.|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|Обеспечивает отображение диапазона в отфильтрованном диапазоне.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|string|Представляет ссылку на диапазон в стиле A1. Значение адреса будет содержать ссылку на лист (например, Лист1!A1:B4). Только для чтения.|
|addressLocal|string|Представляет ссылку на указанный диапазон на языке пользователя. Только для чтения.|
|cellCount|int|Количество ячеек в диапазоне. Только для чтения.|
|columnCount|int|Представляет общее количество столбцов в диапазоне. Только для чтения.|
|columnHidden|boolean|Указывает, скрыты ли все столбцы текущего диапазона.|
|columnIndex|int|Представляет номер столбца первой ячейки диапазона. Используется нулевой индекс. Только для чтения.|
|formulas|Json|Представляет формулу в формате A1.|
|formulasLocal|Json|Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.|
|formulasR1C1|Json|Представляет формулу в формате R1C1.|
|hidden|boolean|Указывает, скрыты ли все ячейки текущего диапазона. Только для чтения.|
|numberFormat|Json|Представляет код в числовом формате Excel для данной ячейки.|
|rowCount|int|Возвращает общее количество строк в диапазоне. Только для чтения.|
|rowHidden|boolean|Указывает, скрыты ли все строки текущего диапазона.|
|rowIndex|int|Возвращает номер строки первой ячейки диапазона. Используется нулевой индекс. Только для чтения.|
|текст|Json|Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.|
|valueTypes|string|Представляет тип данных каждой ячейки. Возможные значения: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукранжеформат](workbookrangeformat.md)|Возвращает объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона. Только для чтения.|
|sort|[воркбукранжесорт](workbookrangesort.md)|Лист, содержащий текущий диапазон. Только для чтения.|
|worksheet|[воркбукворкшит](workbookworksheet.md)|Лист, содержащий текущий диапазон. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRange"
}-->

```json
{
  "id": "string",
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "hidden": true,
  "numberFormat": "Json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "Json",
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
  "suppressions": []
}
-->
