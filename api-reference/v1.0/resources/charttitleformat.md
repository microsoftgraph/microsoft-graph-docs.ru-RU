---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c3632c381dcd29247696c50bc235b9662c8d6366
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032888"
---
# <a name="charttitleformat-resource-type"></a>Тип ресурса ChartTitleFormat

Инкапсулирует свойства формата для заголовка диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[Воркбукчартфилл](chartfill.md)|Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.|
|font|[Воркбукчартфонт](chartfont.md)|Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта. Только для чтения.|



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
