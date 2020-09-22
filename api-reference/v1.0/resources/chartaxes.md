---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5f647e40c2d4d5f3ab3b5206a4b172f70463c2ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032798"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="d5e0a-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="d5e0a-103">ChartAxes resource type</span></span>

<span data-ttu-id="d5e0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5e0a-105">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="d5e0a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d5e0a-106">Methods</span></span>
<span data-ttu-id="d5e0a-107">Нет</span><span class="sxs-lookup"><span data-stu-id="d5e0a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="d5e0a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5e0a-108">Properties</span></span>
<span data-ttu-id="d5e0a-109">Нет</span><span class="sxs-lookup"><span data-stu-id="d5e0a-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d5e0a-110">Связи</span><span class="sxs-lookup"><span data-stu-id="d5e0a-110">Relationships</span></span>
| <span data-ttu-id="d5e0a-111">Связь</span><span class="sxs-lookup"><span data-stu-id="d5e0a-111">Relationship</span></span> | <span data-ttu-id="d5e0a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d5e0a-112">Type</span></span>   |<span data-ttu-id="d5e0a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e0a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e0a-114">категоряксис</span><span class="sxs-lookup"><span data-stu-id="d5e0a-114">categoryAxis</span></span>|[<span data-ttu-id="d5e0a-115">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="d5e0a-115">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d5e0a-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="d5e0a-118">сериесаксис</span><span class="sxs-lookup"><span data-stu-id="d5e0a-118">seriesAxis</span></span>|[<span data-ttu-id="d5e0a-119">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="d5e0a-119">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d5e0a-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="d5e0a-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="d5e0a-122">valueAxis</span></span>|[<span data-ttu-id="d5e0a-123">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="d5e0a-123">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d5e0a-124">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="d5e0a-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5e0a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5e0a-126">JSON representation</span></span>

<span data-ttu-id="d5e0a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5e0a-127">Here is a JSON representation of the resource.</span></span>

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

