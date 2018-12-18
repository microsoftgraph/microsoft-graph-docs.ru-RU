---
title: Тип ресурса ChartAxisFormat
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
ms.openlocfilehash: e503b4e62ef7907943f10a395f12eb5d86c1928f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359460"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="d6fba-103">Тип ресурса ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="d6fba-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="d6fba-104">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d6fba-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="d6fba-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d6fba-105">Methods</span></span>
<span data-ttu-id="d6fba-106">Нет</span><span class="sxs-lookup"><span data-stu-id="d6fba-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="d6fba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6fba-107">Properties</span></span>
<span data-ttu-id="d6fba-108">Нет</span><span class="sxs-lookup"><span data-stu-id="d6fba-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d6fba-109">Связи</span><span class="sxs-lookup"><span data-stu-id="d6fba-109">Relationships</span></span>
| <span data-ttu-id="d6fba-110">Связь</span><span class="sxs-lookup"><span data-stu-id="d6fba-110">Relationship</span></span> | <span data-ttu-id="d6fba-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d6fba-111">Type</span></span>   |<span data-ttu-id="d6fba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d6fba-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6fba-113">font</span><span class="sxs-lookup"><span data-stu-id="d6fba-113">font</span></span>|[<span data-ttu-id="d6fba-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d6fba-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d6fba-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6fba-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="d6fba-117">line</span><span class="sxs-lookup"><span data-stu-id="d6fba-117">line</span></span>|[<span data-ttu-id="d6fba-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d6fba-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="d6fba-p102">Представляет форматирование линий диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6fba-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d6fba-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6fba-121">JSON representation</span></span>

<span data-ttu-id="d6fba-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6fba-122">Here is a JSON representation of the resource.</span></span>

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