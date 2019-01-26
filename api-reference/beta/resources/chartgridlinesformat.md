---
title: Тип ресурса ChartGridlinesFormat
description: Инкапсулирует свойства формата для линий сетки диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf2e9f1202774cc971cc09a2ce1904df2e1fb5a2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573286"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="6f249-103">Тип ресурса ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="6f249-103">ChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f249-104">Инкапсулирует свойства формата для линий сетки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6f249-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="6f249-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6f249-105">Methods</span></span>
<span data-ttu-id="6f249-106">Нет</span><span class="sxs-lookup"><span data-stu-id="6f249-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6f249-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f249-107">Properties</span></span>
<span data-ttu-id="6f249-108">Нет</span><span class="sxs-lookup"><span data-stu-id="6f249-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6f249-109">Связи</span><span class="sxs-lookup"><span data-stu-id="6f249-109">Relationships</span></span>
| <span data-ttu-id="6f249-110">Связь</span><span class="sxs-lookup"><span data-stu-id="6f249-110">Relationship</span></span> | <span data-ttu-id="6f249-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6f249-111">Type</span></span>   |<span data-ttu-id="6f249-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6f249-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f249-113">line</span><span class="sxs-lookup"><span data-stu-id="6f249-113">line</span></span>|[<span data-ttu-id="6f249-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6f249-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="6f249-p101">Представляет форматирование линий диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f249-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6f249-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f249-117">JSON representation</span></span>

<span data-ttu-id="6f249-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f249-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlinesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
