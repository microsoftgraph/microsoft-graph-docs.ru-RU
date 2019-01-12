---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 48d6cb0d35e82fc0117a24aad1c5e171bc869870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961419"
---
# <a name="chartdatalabels-resource-type"></a>Тип ресурса ChartDataLabels

Представляет коллекцию всех меток данных в точке диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartDataLabels](../api/chartdatalabels-get.md) | [WorkbookChartDataLabels](chartdatalabels.md) |Чтение свойств и связей объекта chartDataLabels.|
|[обновление](../api/chartdatalabels-update.md). | [WorkbookChartDataLabels](chartdatalabels.md) |Обновление объекта chartDataLabels. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|position|string|DataLabelPosition значение, представляющее положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.|
|разделитель|string|Строка, представляющая разделитель для меток данных на диаграмме.|
|showBubbleSize|boolean|Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.|
|showCategoryName|boolean|Логическое значение, которое указывает, отображается ли имя для категории меток данных.|
|showLegendKey|boolean|Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.|
|showPercentage|boolean|Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.|
|showSeriesName|boolean|Логическое значение, которое указывает, отображается ли имя ряда для меток данных.|
|showValue|boolean|Логическое значение, которое указывает, отображается ли значение метки данных.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartDataLabelFormat](chartdatalabelformat.md)|Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
