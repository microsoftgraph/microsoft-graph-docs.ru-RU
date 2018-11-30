---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
ms.openlocfilehash: 4fc801ecdba147a26b30f07a2487eabe11acfb3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025314"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="cd7ff-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="cd7ff-103">ChartAxes resource type</span></span>

<span data-ttu-id="cd7ff-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="cd7ff-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="cd7ff-105">Методы</span><span class="sxs-lookup"><span data-stu-id="cd7ff-105">Methods</span></span>
<span data-ttu-id="cd7ff-106">Нет</span><span class="sxs-lookup"><span data-stu-id="cd7ff-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="cd7ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd7ff-107">Properties</span></span>
<span data-ttu-id="cd7ff-108">Нет</span><span class="sxs-lookup"><span data-stu-id="cd7ff-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cd7ff-109">Связи</span><span class="sxs-lookup"><span data-stu-id="cd7ff-109">Relationships</span></span>
| <span data-ttu-id="cd7ff-110">Связь</span><span class="sxs-lookup"><span data-stu-id="cd7ff-110">Relationship</span></span> | <span data-ttu-id="cd7ff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cd7ff-111">Type</span></span>   |<span data-ttu-id="cd7ff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd7ff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd7ff-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-113">categoryAxis</span></span>|[<span data-ttu-id="cd7ff-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd7ff-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd7ff-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="cd7ff-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-117">seriesAxis</span></span>|[<span data-ttu-id="cd7ff-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd7ff-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd7ff-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="cd7ff-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-121">valueAxis</span></span>|[<span data-ttu-id="cd7ff-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd7ff-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd7ff-p103">Представляет ось значений для оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd7ff-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd7ff-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd7ff-125">JSON representation</span></span>

<span data-ttu-id="cd7ff-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd7ff-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->