---
title: Тип ресурса Воркбукчартпоинт
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12cc2f9a700ef66ec47a72aa88a2c30f2c2c3f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349003"
---
# <a name="workbookchartpoint-resource-type"></a>Тип ресурса Воркбукчартпоинт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет точку из ряда в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукчартпоинт](../api/chartpoint-get.md) | [Воркбукчартпоинт](workbookchartpoint.md) |Чтение свойств и связей объекта chartPoint.|
|[Список](../api/chartpoint-list.md) | Коллекция [воркбукчартпоинт](workbookchartpoint.md) |Получение коллекции объектов chartPoint. |
|[Итемат](../api/chartpointscollection-itemat.md)|[Воркбукчартпоинт](workbookchartpoint.md)|Получение точки на основании ее положения в ряду.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|значение|Json|Возвращает значение точки диаграммы. Только для чтения.|
|id|string|уникальный идентификатор|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[Воркбукчартпоинтформат](workbookchartpointformat.md)|Инкапсулирует свойства формата точки диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
