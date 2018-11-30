---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027739"
---
# <a name="chartpoint-resource-type"></a>Тип ресурса ChartPoint

Представляет точку из ряда в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartPoint](../api/chartpoint-get.md) | [WorkbookChartPoint](chartpoint.md) |Чтение свойств и связей объекта chartPoint.|
|[List](../api/chartpoint-list.md) | [WorkbookChartPoint](chartpoint.md) коллекции |Получение коллекции объектов chartPoint. |
|[ItemAt](../api/chartpointscollection-itemat.md)|[WorkbookChartPoint](chartpoint.md)|Получение точки на основании ее положения в ряду.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|value|Json|Возвращает значение точки диаграммы. Только для чтения.|
|id|строка|Уникальный идентификатор|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartPointFormat](chartpointformat.md)|Инкапсулирует свойства формата точки диаграммы. Только для чтения.|

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