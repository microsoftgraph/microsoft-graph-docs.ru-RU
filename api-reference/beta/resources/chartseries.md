---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5a299c7140c2032a57cd47fb0880ae34620a920b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915818"
---
# <a name="chartseries-resource-type"></a>Тип ресурса ChartSeries

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [ChartSeries](chartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание объекта ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Создание объекта ChartPoints путем добавления в коллекцию точек.|
|[Список точек](../api/chartseries-list-points.md) |Коллекция объектов [ChartPoints](chartpoint.md)| Получение коллекции объектов ChartPoints.|
|[обновление](../api/chartseries-update.md). | [ChartSeries](chartseries.md) |Обновление объекта ChartSeries. |
|[List](../api/chartseries-list.md) | Коллекция объектов [ChartSeries](chartseries.md) |Получение коллекции объектов chartSeries. |
|[Itemat](../api/chartseriescollection-itemat.md)|[ChartSeries](chartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|строка|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[ChartSeriesFormat](chartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|Коллекция объектов [ChartPoints](chartpoint.md)|Представляет коллекцию всех точек в ряду. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
