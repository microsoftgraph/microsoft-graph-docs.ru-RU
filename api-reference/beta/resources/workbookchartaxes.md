---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15e63af1e7b648288dba813790302f1dee6536ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348946"
---
# <a name="workbookchartaxes-resource-type"></a>Тип ресурса Воркбукчартаксес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет оси диаграммы.


## <a name="methods"></a>Методы
Отсутствует

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
