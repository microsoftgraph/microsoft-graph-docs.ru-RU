---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9b79f437e2c739c675533e9178ddcbb3da21b922
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049678"
---
# <a name="chartlegend-resource-type"></a>Тип ресурса ChartLegend

Пространство имен: microsoft.graph

Представляет легенду в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartLegend](../api/chartlegend-get.md) | [КнигаChartLegend](chartlegend.md) |Чтение свойств и связей объекта chartLegend.|
|[Обновление](../api/chartlegend-update.md) | [КнигаChartLegend](chartlegend.md) |Обновление объекта ChartLegend. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|overlay|boolean|Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.|
|position|string|Представляет расположение легенды на диаграмме. Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.|
|visible|boolean|Логическое значение, представляющее видимость объекта ChartLegend.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartLegendFormat](chartlegendformat.md)|Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

