---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7d743695c6d7cd94636a795f75a8059976f743e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032400"
---
# <a name="chartaxes-resource-type"></a>Тип ресурса ChartAxes

Пространство имен: microsoft.graph

Представляет оси диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryAxis|[КнигаChartAxis](chartaxis.md)|Представляет ось категорий на диаграмме. Только для чтения.|
|seriesAxis|[КнигаChartAxis](chartaxis.md)|Представляет ось ряда данных для объемной диаграммы. Только для чтения.|
|valueAxis|[КнигаChartAxis](chartaxis.md)|Представляет ось значений для оси. Только для чтения.|

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

