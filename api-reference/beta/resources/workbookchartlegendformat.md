---
title: Тип ресурса Воркбукчартлежендформат
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 32f9fcec2002039c9ccee399c90f1a26048c71cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519304"
---
# <a name="workbookchartlegendformat-resource-type"></a>Тип ресурса Воркбукчартлежендформат

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инкапсулирует свойства формата легенды диаграммы.

## <a name="methods"></a>Methods
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[воркбукчартфилл](workbookchartfill.md)|Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.|
|шрифт|[воркбукчартфонт](workbookchartfont.md)|Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
