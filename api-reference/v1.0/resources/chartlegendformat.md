---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2148b6b5baf8bb680f85954d000da097bcf8f0b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032958"
---
# <a name="chartlegendformat-resource-type"></a>Тип ресурса ChartLegendFormat

Инкапсулирует свойства формата легенды диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[Воркбукчартфилл](chartfill.md)|Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.|
|шрифт|[Воркбукчартфонт](chartfont.md)|Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
