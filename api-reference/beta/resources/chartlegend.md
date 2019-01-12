---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c76fd21700616ec6c353644de93bddd0a47ac7dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980883"
---
# <a name="chartlegend-resource-type"></a>Тип ресурса ChartLegend

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет легенду в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartLegend](../api/chartlegend-get.md) | [ChartLegend](chartlegend.md) |Чтение свойств и связей объекта chartLegend.|
|[обновление](../api/chartlegend-update.md). | [ChartLegend](chartlegend.md) |Обновление объекта ChartLegend. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|overlay|boolean|Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.|
|position|string|Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.|
|visible|boolean|Логическое значение, представляющее видимость объекта ChartLegend.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[ChartLegendFormat](chartlegendformat.md)|Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
