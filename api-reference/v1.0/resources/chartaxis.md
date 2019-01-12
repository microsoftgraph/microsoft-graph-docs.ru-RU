---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88066c356306a619ee620a13eefb6592d7b5f100
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984313"
---
# <a name="chartaxis-resource-type"></a>Тип ресурса ChartAxis

Представляет одну ось на диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartAxis](../api/chartaxis-get.md) | [WorkbookChartAxis](chartaxis.md) |Чтение свойств и связей объекта chartAxis.|
|[обновление](../api/chartaxis-update.md). | [WorkbookChartAxis](chartaxis.md)   |Обновление объекта ChartAxis. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id       |строка   | Уникальный идентификатор. Только для чтения.|
|majorUnit|Json|Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.|
|maximum|Json|Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.|
|minimum|Json|Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.|
|minorUnit|Json|Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartAxisFormat](chartaxisformat.md)|Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.|
|majorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.|
|minorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.|
|должности.|[WorkbookChartAxisTitle](chartaxistitle.md)|Представляет название оси. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
