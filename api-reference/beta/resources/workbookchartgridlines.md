---
title: Тип ресурса Воркбукчартгридлинес
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dce652981a16445d82b4d6e556fc7d5ce839ed26
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348997"
---
# <a name="workbookchartgridlines-resource-type"></a>Тип ресурса Воркбукчартгридлинес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет основные или вспомогательные линии сетки на оси диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукчартгридлинес](../api/chartgridlines-get.md) | [Воркбукчартгридлинес](workbookchartgridlines.md) |Чтение свойств и связей объекта chartGridlines.|
|[Обновление](../api/chartgridlines-update.md) | [Воркбукчартгридлинес](workbookchartgridlines.md)    |Обновление объекта ChartGridlines. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|visible|boolean|Логическое значение, определяющее, отображаются ли линии сетки оси.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[Воркбукчартгридлинесформат](workbookchartgridlinesformat.md)|Представляет форматирование линий сетки диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
