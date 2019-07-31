---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e7cd34ab250f5232d1620af3b3be4fe36c286f41
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964085"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="c888d-103">Тип ресурса Воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="c888d-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c888d-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c888d-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="c888d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c888d-105">Methods</span></span>
<span data-ttu-id="c888d-106">Нет</span><span class="sxs-lookup"><span data-stu-id="c888d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c888d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c888d-107">Properties</span></span>
<span data-ttu-id="c888d-108">Нет</span><span class="sxs-lookup"><span data-stu-id="c888d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c888d-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="c888d-109">Relationships</span></span>
| <span data-ttu-id="c888d-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="c888d-110">Relationship</span></span> | <span data-ttu-id="c888d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c888d-111">Type</span></span>   |<span data-ttu-id="c888d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c888d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c888d-113">Категоряксис</span><span class="sxs-lookup"><span data-stu-id="c888d-113">categoryAxis</span></span>|[<span data-ttu-id="c888d-114">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c888d-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="c888d-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c888d-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="c888d-117">Сериесаксис</span><span class="sxs-lookup"><span data-stu-id="c888d-117">seriesAxis</span></span>|[<span data-ttu-id="c888d-118">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c888d-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="c888d-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c888d-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="c888d-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="c888d-121">valueAxis</span></span>|[<span data-ttu-id="c888d-122">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="c888d-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="c888d-123">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="c888d-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="c888d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c888d-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c888d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c888d-125">JSON representation</span></span>

<span data-ttu-id="c888d-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c888d-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
