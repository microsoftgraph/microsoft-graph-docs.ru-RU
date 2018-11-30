---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
ms.openlocfilehash: ec81523dc09c17cd8c7fb9d543c2214377201260
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025402"
---
# <a name="chartdatalabelformat-resource-type"></a>Тип ресурса ChartDataLabelFormat

Инкапсулирует свойства формата для меток данных диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.|
|font|[WorkbookChartFont](chartfont.md)|Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для метки данных диаграммы. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->