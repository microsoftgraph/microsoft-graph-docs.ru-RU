---
title: Тип ресурса ChartAxes
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569433"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="c10d5-103">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="c10d5-103">ChartAxes resource type</span></span>

<span data-ttu-id="c10d5-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c10d5-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="c10d5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c10d5-105">Methods</span></span>
<span data-ttu-id="c10d5-106">Нет</span><span class="sxs-lookup"><span data-stu-id="c10d5-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c10d5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c10d5-107">Properties</span></span>
<span data-ttu-id="c10d5-108">Нет</span><span class="sxs-lookup"><span data-stu-id="c10d5-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c10d5-109">Связи</span><span class="sxs-lookup"><span data-stu-id="c10d5-109">Relationships</span></span>
| <span data-ttu-id="c10d5-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="c10d5-110">Relationship</span></span> | <span data-ttu-id="c10d5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c10d5-111">Type</span></span>   |<span data-ttu-id="c10d5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c10d5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c10d5-113">Категоряксис</span><span class="sxs-lookup"><span data-stu-id="c10d5-113">categoryAxis</span></span>|[<span data-ttu-id="c10d5-114">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c10d5-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c10d5-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c10d5-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="c10d5-117">Сериесаксис</span><span class="sxs-lookup"><span data-stu-id="c10d5-117">seriesAxis</span></span>|[<span data-ttu-id="c10d5-118">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c10d5-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c10d5-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c10d5-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="c10d5-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="c10d5-121">valueAxis</span></span>|[<span data-ttu-id="c10d5-122">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c10d5-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c10d5-123">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="c10d5-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="c10d5-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c10d5-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c10d5-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c10d5-125">JSON representation</span></span>

<span data-ttu-id="c10d5-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c10d5-126">Here is a JSON representation of the resource.</span></span>

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
