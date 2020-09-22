---
title: Тип ресурса Воркбукчартдаталабелс
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 28dc0d70f057569cd240770e15964b13c7982bae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979289"
---
# <a name="workbookchartdatalabels-resource-type"></a>Тип ресурса Воркбукчартдаталабелс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию всех меток данных в точке диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукчартдаталабелс](../api/chartdatalabels-get.md) | [воркбукчартдаталабелс](workbookchartdatalabels.md) |Чтение свойств и связей объекта chartDataLabels.|
|[Обновление](../api/chartdatalabels-update.md) | [воркбукчартдаталабелс](workbookchartdatalabels.md) |Обновление объекта chartDataLabels. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|position|string|Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None` , `Center` ,,, `InsideEnd` `InsideBase` `OutsideEnd` , `Left` , `Right` ,,, `Top` `Bottom` `BestFit` , `Callout` .|
|separator|string|Строка, представляющая разделитель для меток данных на диаграмме.|
|showBubbleSize|boolean|Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.|
|showCategoryName|boolean|Логическое значение, которое указывает, отображается ли имя для категории меток данных.|
|showLegendKey|boolean|Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.|
|showPercentage|boolean|Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.|
|showSeriesName|boolean|Логическое значение, которое указывает, отображается ли имя ряда для меток данных.|
|showValue|boolean|Логическое значение, которое указывает, отображается ли значение метки данных.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукчартдаталабелформат](workbookchartdatalabelformat.md)|Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.|

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


