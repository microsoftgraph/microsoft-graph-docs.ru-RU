---
title: Тип ресурса Воркбукчартсериес
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 22ce2138da7ae8163304978370ada1f71abe7026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979233"
---
# <a name="workbookchartseries-resource-type"></a>Тип ресурса Воркбукчартсериес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries-get.md) | [воркбукчартсериес](workbookchartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание ChartPoint](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| Создание нового chartPoint путем публикации в коллекции Points.|
|[Список точек](../api/chartseries-list-points.md) |Коллекция [воркбукчартпоинтс](workbookchartpoint.md)| Получение коллекции объектов chartPoints.|
|[обновление](../api/chartseries-update.md). | [воркбукчартсериес](workbookchartseries.md) |Обновление объекта chartSeries. |
|[List](../api/chartseries-list.md) | Коллекция [воркбукчартсериес](workbookchartseries.md) |Получение коллекции объектов chartSeries. |
|[итемат](../api/chartseriescollection-itemat.md)|[воркбукчартсериес](workbookchartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукчартсериесформат](workbookchartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
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


