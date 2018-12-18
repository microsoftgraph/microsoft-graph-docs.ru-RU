---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
ms.openlocfilehash: 39c95d0849d398df7d57f676cc392c157e6f43f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339055"
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