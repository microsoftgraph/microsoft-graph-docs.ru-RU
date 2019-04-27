---
title: Тип ресурса Воркбукчартсериес
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348981"
---
# <a name="workbookchartseries-resource-type"></a>Тип ресурса Воркбукчартсериес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [Воркбукчартсериес](workbookchartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание ChartPoint](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| Создание нового chartPoint путем публикации в коллекции Points.|
|[Список точек](../api/chartseries-list-points.md) |Коллекция [воркбукчартпоинтс](workbookchartpoint.md)| Получение коллекции объектов chartPoints.|
|[Обновление](../api/chartseries-update.md) | [Воркбукчартсериес](workbookchartseries.md) |Обновление объекта chartSeries. |
|[Список](../api/chartseries-list.md) | Коллекция [воркбукчартсериес](workbookchartseries.md) |Получение коллекции объектов chartSeries. |
|[Итемат](../api/chartseriescollection-itemat.md)|[Воркбукчартсериес](workbookchartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[Воркбукчартсериесформат](workbookchartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|Коллекция [воркбукчартпоинт](workbookchartpoint.md)|Представляет коллекцию всех точек в ряду. Только для чтения.|

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
  "suppressions": []
}
-->
