---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2a3744e38ffebef0c28784c0fd4be8f35b8af23
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570864"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="f527b-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="f527b-103">ChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f527b-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f527b-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="f527b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f527b-105">Methods</span></span>
<span data-ttu-id="f527b-106">Нет</span><span class="sxs-lookup"><span data-stu-id="f527b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f527b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f527b-107">Properties</span></span>
<span data-ttu-id="f527b-108">Нет</span><span class="sxs-lookup"><span data-stu-id="f527b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f527b-109">Связи</span><span class="sxs-lookup"><span data-stu-id="f527b-109">Relationships</span></span>
| <span data-ttu-id="f527b-110">Связь</span><span class="sxs-lookup"><span data-stu-id="f527b-110">Relationship</span></span> | <span data-ttu-id="f527b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f527b-111">Type</span></span>   |<span data-ttu-id="f527b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f527b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f527b-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-113">categoryAxis</span></span>|[<span data-ttu-id="f527b-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f527b-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f527b-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="f527b-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-117">seriesAxis</span></span>|[<span data-ttu-id="f527b-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f527b-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f527b-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="f527b-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-121">valueAxis</span></span>|[<span data-ttu-id="f527b-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f527b-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f527b-p103">Представляет ось значений для оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f527b-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f527b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f527b-125">JSON representation</span></span>

<span data-ttu-id="f527b-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f527b-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
