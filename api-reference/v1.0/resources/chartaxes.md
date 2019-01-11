---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 53f0e4a7344ddfab89330203f90032266e0c622d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885906"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="7c1a2-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="7c1a2-103">ChartAxes resource type</span></span>

<span data-ttu-id="7c1a2-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="7c1a2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7c1a2-105">Methods</span></span>
<span data-ttu-id="7c1a2-106">Нет</span><span class="sxs-lookup"><span data-stu-id="7c1a2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7c1a2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c1a2-107">Properties</span></span>
<span data-ttu-id="7c1a2-108">Нет</span><span class="sxs-lookup"><span data-stu-id="7c1a2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7c1a2-109">Связи</span><span class="sxs-lookup"><span data-stu-id="7c1a2-109">Relationships</span></span>
| <span data-ttu-id="7c1a2-110">Связь</span><span class="sxs-lookup"><span data-stu-id="7c1a2-110">Relationship</span></span> | <span data-ttu-id="7c1a2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7c1a2-111">Type</span></span>   |<span data-ttu-id="7c1a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7c1a2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c1a2-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-113">categoryAxis</span></span>|[<span data-ttu-id="7c1a2-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="7c1a2-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="7c1a2-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-117">seriesAxis</span></span>|[<span data-ttu-id="7c1a2-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="7c1a2-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="7c1a2-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-121">valueAxis</span></span>|[<span data-ttu-id="7c1a2-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="7c1a2-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="7c1a2-p103">Представляет ось значений для оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c1a2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c1a2-125">JSON representation</span></span>

<span data-ttu-id="7c1a2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-126">Here is a JSON representation of the resource.</span></span>

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
