---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: befa6f552fd343140d2aae10266c1445066266d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531833"
---
# <a name="chartpoint-resource-type"></a>Тип ресурса ChartPoint

Пространство имен: microsoft.graph

Представляет точку из ряда в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartPoint](../api/chartpoint-get.md) | [воркбукчартпоинт](chartpoint.md) |Чтение свойств и связей объекта chartPoint.|
|[Список](../api/chartpoint-list.md) | Коллекция [воркбукчартпоинт](chartpoint.md) |Получение коллекции объектов chartPoint. |
|[итемат](../api/chartpointscollection-itemat.md)|[воркбукчартпоинт](chartpoint.md)|Получение точки на основании ее положения в ряду.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|значение|Json|Возвращает значение точки диаграммы. Только для чтения.|
|id|string|уникальный идентификатор|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукчартпоинтформат](chartpointformat.md)|Инкапсулирует свойства формата точки диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
