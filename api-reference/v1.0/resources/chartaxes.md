---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7e8ee5eac8face4d16418799d627d3aa168c48c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029878"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="9f7c2-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="9f7c2-103">ChartAxes resource type</span></span>

<span data-ttu-id="9f7c2-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="9f7c2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9f7c2-105">Methods</span></span>
<span data-ttu-id="9f7c2-106">Нет</span><span class="sxs-lookup"><span data-stu-id="9f7c2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9f7c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f7c2-107">Properties</span></span>
<span data-ttu-id="9f7c2-108">Нет</span><span class="sxs-lookup"><span data-stu-id="9f7c2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9f7c2-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="9f7c2-109">Relationships</span></span>
| <span data-ttu-id="9f7c2-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="9f7c2-110">Relationship</span></span> | <span data-ttu-id="9f7c2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9f7c2-111">Type</span></span>   |<span data-ttu-id="9f7c2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9f7c2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f7c2-113">Категоряксис</span><span class="sxs-lookup"><span data-stu-id="9f7c2-113">categoryAxis</span></span>|[<span data-ttu-id="9f7c2-114">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="9f7c2-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9f7c2-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="9f7c2-117">Сериесаксис</span><span class="sxs-lookup"><span data-stu-id="9f7c2-117">seriesAxis</span></span>|[<span data-ttu-id="9f7c2-118">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="9f7c2-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9f7c2-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="9f7c2-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="9f7c2-121">valueAxis</span></span>|[<span data-ttu-id="9f7c2-122">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="9f7c2-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9f7c2-123">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="9f7c2-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f7c2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f7c2-125">JSON representation</span></span>

<span data-ttu-id="9f7c2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f7c2-126">Here is a JSON representation of the resource.</span></span>

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
