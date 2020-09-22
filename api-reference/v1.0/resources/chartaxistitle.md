---
title: Тип ресурса ChartAxisTitle
description: Представляет название оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f43e780a6a574b465f293f432cb4581d645bba3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069206"
---
# <a name="chartaxistitle-resource-type"></a>Тип ресурса ChartAxisTitle

Пространство имен: microsoft.graph

Представляет название оси диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartAxisTitle](../api/chartaxistitle-get.md) | [воркбукчартаксиститле](chartaxistitle.md) |Чтение свойств и связей объекта chartAxisTitle.|
|[Обновление](../api/chartaxistitle-update.md) | [воркбукчартаксиститле](chartaxistitle.md)    |Обновление объекта ChartAxisTitle. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|text|string|Обозначает название оси.|
|visible|boolean|Логическое значение, которое определяет видимость названия оси.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукчартаксиститлеформат](chartaxistitleformat.md)|Представляет форматирование для названия оси диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

