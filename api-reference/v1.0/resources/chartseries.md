---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b9a857f127848f1ed0da8de673902527e3858ffe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569041"
---
# <a name="chartseries-resource-type"></a>Тип ресурса ChartSeries

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [Воркбукчартсериес](chartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание объекта ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Создание объекта ChartPoints путем добавления в коллекцию точек.|
|[Список точек](../api/chartseries-list-points.md) |Коллекция объектов [ChartPoints](chartpoint.md)| Получение коллекции объектов ChartPoints.|
|[Обновление](../api/chartseries-update.md) | [Воркбукчартсериес](chartseries.md) |Обновление объекта ChartSeries. |
|[Список](../api/chartseries-list.md) | Коллекция [воркбукчартсериес](chartseries.md) |Получение коллекции объектов chartSeries. |
|[Итемат](../api/chartseriescollection-itemat.md)|[Воркбукчартсериес](chartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[Воркбукчартсериесформат](chartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|Коллекция [воркбукчартпоинт](chartpoint.md)|Представляет коллекцию всех точек в ряду. Только для чтения.|

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
