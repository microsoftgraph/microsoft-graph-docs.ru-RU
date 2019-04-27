---
title: Тип ресурса Воркбукчарттитлеформат
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3827b44ae24a63f8fe048575633cc3b5508ac300
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348998"
---
# <a name="workbookcharttitleformat-resource-type"></a>Тип ресурса Воркбукчарттитлеформат

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инкапсулирует свойства формата для заголовка диаграммы.


## <a name="methods"></a>Методы
Отсутствует

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fill|[Воркбукчартфилл](workbookchartfill.md)|Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.|
|font|[Воркбукчартфонт](workbookchartfont.md)|Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта. Только для чтения.|



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "workbookChartTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
