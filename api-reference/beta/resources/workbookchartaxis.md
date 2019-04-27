---
title: Тип ресурса Воркбукчартаксис
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ce18f029e3e5e48597ac5074d683e6a8cdb64674
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348945"
---
# <a name="workbookchartaxis-resource-type"></a>Тип ресурса Воркбукчартаксис

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одну ось на диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartAxis](../api/chartaxis-get.md) | [Воркбукчартаксис](workbookchartaxis.md) |Чтение свойств и связей объекта chartAxis.|
|[Обновление](../api/chartaxis-update.md) | [Воркбукчартаксис](workbookchartaxis.md)   |Обновление объекта ChartAxis. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id       |string   | Уникальный идентификатор. Только для чтения.|
|majorUnit|Json|Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.|
|maximum|Json|Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.|
|minimum|Json|Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.|
|minorUnit|Json|Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[Воркбукчартаксисформат](workbookchartaxisformat.md)|Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.|
|majorGridlines|[Воркбукчартгридлинес](workbookchartgridlines.md)|Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.|
|minorGridlines|[Воркбукчартгридлинес](workbookchartgridlines.md)|Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.|
|title|[Воркбукчартаксиститле](workbookchartaxistitle.md)|Обозначает название оси. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
