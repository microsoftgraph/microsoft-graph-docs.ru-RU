---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a5a33108de8225e3222ecea74afa3c0d9f1caa4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531911"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="fc293-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="fc293-103">ChartAxes resource type</span></span>

<span data-ttu-id="fc293-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc293-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc293-105">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="fc293-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="fc293-106">Methods</span><span class="sxs-lookup"><span data-stu-id="fc293-106">Methods</span></span>
<span data-ttu-id="fc293-107">Нет</span><span class="sxs-lookup"><span data-stu-id="fc293-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="fc293-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc293-108">Properties</span></span>
<span data-ttu-id="fc293-109">Нет</span><span class="sxs-lookup"><span data-stu-id="fc293-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fc293-110">Связи</span><span class="sxs-lookup"><span data-stu-id="fc293-110">Relationships</span></span>
| <span data-ttu-id="fc293-111">Связь</span><span class="sxs-lookup"><span data-stu-id="fc293-111">Relationship</span></span> | <span data-ttu-id="fc293-112">Тип</span><span class="sxs-lookup"><span data-stu-id="fc293-112">Type</span></span>   |<span data-ttu-id="fc293-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fc293-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc293-114">категоряксис</span><span class="sxs-lookup"><span data-stu-id="fc293-114">categoryAxis</span></span>|[<span data-ttu-id="fc293-115">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="fc293-115">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc293-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc293-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="fc293-118">сериесаксис</span><span class="sxs-lookup"><span data-stu-id="fc293-118">seriesAxis</span></span>|[<span data-ttu-id="fc293-119">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="fc293-119">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc293-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc293-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="fc293-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="fc293-122">valueAxis</span></span>|[<span data-ttu-id="fc293-123">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="fc293-123">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc293-124">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="fc293-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="fc293-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc293-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc293-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc293-126">JSON representation</span></span>

<span data-ttu-id="fc293-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc293-127">Here is a JSON representation of the resource.</span></span>

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
