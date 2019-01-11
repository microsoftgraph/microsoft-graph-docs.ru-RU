---
title: Тип ресурса ChartAxisFormat
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a219122141da1f384279d0ff4c612f62226612c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821268"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="991d3-103">Тип ресурса ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="991d3-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="991d3-104">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="991d3-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="991d3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="991d3-105">Methods</span></span>
<span data-ttu-id="991d3-106">Нет</span><span class="sxs-lookup"><span data-stu-id="991d3-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="991d3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="991d3-107">Properties</span></span>
<span data-ttu-id="991d3-108">Нет</span><span class="sxs-lookup"><span data-stu-id="991d3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="991d3-109">Связи</span><span class="sxs-lookup"><span data-stu-id="991d3-109">Relationships</span></span>
| <span data-ttu-id="991d3-110">Связь</span><span class="sxs-lookup"><span data-stu-id="991d3-110">Relationship</span></span> | <span data-ttu-id="991d3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="991d3-111">Type</span></span>   |<span data-ttu-id="991d3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="991d3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="991d3-113">font</span><span class="sxs-lookup"><span data-stu-id="991d3-113">font</span></span>|[<span data-ttu-id="991d3-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="991d3-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="991d3-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="991d3-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="991d3-117">line</span><span class="sxs-lookup"><span data-stu-id="991d3-117">line</span></span>|[<span data-ttu-id="991d3-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="991d3-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="991d3-p102">Представляет форматирование линий диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="991d3-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="991d3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="991d3-121">JSON representation</span></span>

<span data-ttu-id="991d3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="991d3-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
