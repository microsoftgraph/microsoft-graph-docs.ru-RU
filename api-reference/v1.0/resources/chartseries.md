---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a3a19793629a5e100830565e224541930e2180de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834897"
---
# <a name="chartseries-resource-type"></a>Тип ресурса ChartSeries

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [WorkbookChartSeries](chartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание объекта ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Создание объекта ChartPoints путем добавления в коллекцию точек.|
|[Список точек](../api/chartseries-list-points.md) |Коллекция объектов [ChartPoints](chartpoint.md)| Получение коллекции объектов ChartPoints.|
|[обновление](../api/chartseries-update.md). | [WorkbookChartSeries](chartseries.md) |Обновление объекта ChartSeries. |
|[List](../api/chartseries-list.md) | [WorkbookChartSeries](chartseries.md) коллекции |Получение коллекции объектов chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[WorkbookChartSeries](chartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|строка|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|[WorkbookChartPoint](chartpoint.md) коллекции|Представляет коллекцию всех точек в ряду. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
