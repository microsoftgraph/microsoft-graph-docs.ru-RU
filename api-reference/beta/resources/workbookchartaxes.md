---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e7cd34ab250f5232d1620af3b3be4fe36c286f41
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964085"
---
# <a name="workbookchartaxes-resource-type"></a>Тип ресурса Воркбукчартаксес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет оси диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Категоряксис|[Воркбукчартаксис](workbookchartaxis.md)|Представляет ось категорий на диаграмме. Только для чтения.|
|Сериесаксис|[Воркбукчартаксис](workbookchartaxis.md)|Представляет ось ряда данных для объемной диаграммы. Только для чтения.|
|valueAxis|[Воркбукчартаксис](workbookchartaxis.md)|Представляет ось значений для оси. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
