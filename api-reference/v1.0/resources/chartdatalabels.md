---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4a705e27893b0bb2f873fa09e3a07e705aab0823
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049713"
---
# <a name="chartdatalabels-resource-type"></a>Тип ресурса ChartDataLabels

Пространство имен: microsoft.graph

Представляет коллекцию всех меток данных в точке диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartDataLabels](../api/chartdatalabels-get.md) | [КнигаChartDataLabels](chartdatalabels.md) |Чтение свойств и связей объекта chartDataLabels.|
|[Обновление](../api/chartdatalabels-update.md) | [КнигаChartDataLabels](chartdatalabels.md) |Обновление объекта chartDataLabels. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|position|string|Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None` `Center` , , , , , , `InsideEnd` , `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` .|
|separator|string|Строка, представляющая разделитель для меток данных на диаграмме.|
|showBubbleSize|boolean|Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.|
|showCategoryName|boolean|Логическое значение, которое указывает, отображается ли имя для категории меток данных.|
|showLegendKey|boolean|Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.|
|showPercentage|boolean|Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.|
|showSeriesName|boolean|Логическое значение, которое указывает, отображается ли имя ряда для меток данных.|
|showValue|boolean|Логическое значение, которое указывает, отображается ли значение метки данных.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[КнигаChartDataLabelFormat](chartdatalabelformat.md)|Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.|

## <a name="json-representation"></a>Представление в формате JSON

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

