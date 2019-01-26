---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a82e88bd8ba083271a821dc86435b0ce55364cec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572607"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="cec1e-103">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="cec1e-103">ChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cec1e-104">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="cec1e-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="cec1e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="cec1e-105">Methods</span></span>
<span data-ttu-id="cec1e-106">Нет</span><span class="sxs-lookup"><span data-stu-id="cec1e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="cec1e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cec1e-107">Properties</span></span>
<span data-ttu-id="cec1e-108">Нет</span><span class="sxs-lookup"><span data-stu-id="cec1e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cec1e-109">Связи</span><span class="sxs-lookup"><span data-stu-id="cec1e-109">Relationships</span></span>
| <span data-ttu-id="cec1e-110">Связь</span><span class="sxs-lookup"><span data-stu-id="cec1e-110">Relationship</span></span> | <span data-ttu-id="cec1e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cec1e-111">Type</span></span>   |<span data-ttu-id="cec1e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cec1e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cec1e-113">fill</span><span class="sxs-lookup"><span data-stu-id="cec1e-113">fill</span></span>|[<span data-ttu-id="cec1e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="cec1e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="cec1e-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cec1e-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="cec1e-117">font</span><span class="sxs-lookup"><span data-stu-id="cec1e-117">font</span></span>|[<span data-ttu-id="cec1e-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="cec1e-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="cec1e-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cec1e-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cec1e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cec1e-121">JSON representation</span></span>

<span data-ttu-id="cec1e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cec1e-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
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
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabelformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
