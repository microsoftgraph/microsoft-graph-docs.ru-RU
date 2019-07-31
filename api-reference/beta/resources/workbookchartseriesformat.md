---
title: Тип ресурса Воркбукчартсериесформат
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 739a874545047c2ed6927cb4e31d2e006f4e6ba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007167"
---
# <a name="workbookchartseriesformat-resource-type"></a>Тип ресурса Воркбукчартсериесформат

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инкапсулирует свойства формата для ряда диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[Воркбукчартфилл](workbookchartfill.md)|Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.|
|line|[Воркбукчартлинеформат](workbookchartlineformat.md)|Представляет форматирование линий. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
