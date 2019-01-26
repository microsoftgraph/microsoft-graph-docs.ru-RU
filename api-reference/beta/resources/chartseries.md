---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eccd0d970ffeff7b41ceb0f9af810bb7a420d663
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570661"
---
# <a name="chartseries-resource-type"></a>Тип ресурса ChartSeries

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](chartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание объекта ChartPoints](../api/chartseries-post-points.md) |[chartPoints](chartpoint.md)| Создание объекта ChartPoints путем добавления в коллекцию точек.|
|[Список точек](../api/chartseries-list-points.md) |[chartPoints](chartpoint.md) коллекции| Получение коллекции объектов ChartPoints.|
|[Update](../api/chartseries-update.md) | [workbookChartSeries](chartseries.md) |Обновление объекта ChartSeries. |
|[List](../api/chartseries-list.md) | [workbookChartSeries](chartseries.md) коллекции |Получение коллекции объектов chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](chartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|строка|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[workbookChartSeriesFormat](chartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|[workbookChartPoint](chartpoint.md) коллекции|Представляет коллекцию всех точек в ряду. Только для чтения.|

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
