---
title: Тип ресурса Воркбукчартпоинтформат
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0896001fda140ff1d2693b3463c472568f1d28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348980"
---
# <a name="workbookchartpointformat-resource-type"></a>Тип ресурса Воркбукчартпоинтформат

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект форматирования для точек диаграммы.


## <a name="methods"></a>Методы
Отсутствует

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[Воркбукчартфилл](workbookchartfill.md)|Представляет формат заливки диаграммы, включая сведения о форматировании фона. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
