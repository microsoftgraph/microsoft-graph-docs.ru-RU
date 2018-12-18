---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
ms.openlocfilehash: 23a9a5cc1f9eaa9a4ff222cf18f00953d829f88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352978"
---
# <a name="chartaxes-resource-type"></a>Тип ресурса ChartAxes

Представляет оси диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryAxis|[WorkbookChartAxis](chartaxis.md)|Представляет ось категорий на диаграмме. Только для чтения.|
|seriesAxis|[WorkbookChartAxis](chartaxis.md)|Представляет ось ряда данных для объемной диаграммы. Только для чтения.|
|valueAxis|[WorkbookChartAxis](chartaxis.md)|Представляет ось значений для оси. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->