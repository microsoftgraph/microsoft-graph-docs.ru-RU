---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 41bb19e048c27f8c498d809cace15080ec79fb05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039098"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="3cb32-103">Тип ресурса Воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="3cb32-103">workbookChartAxes resource type</span></span>

<span data-ttu-id="3cb32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb32-105">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3cb32-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="3cb32-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3cb32-106">Methods</span></span>
<span data-ttu-id="3cb32-107">Нет</span><span class="sxs-lookup"><span data-stu-id="3cb32-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3cb32-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cb32-108">Properties</span></span>
<span data-ttu-id="3cb32-109">Нет</span><span class="sxs-lookup"><span data-stu-id="3cb32-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3cb32-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="3cb32-110">Relationships</span></span>
| <span data-ttu-id="3cb32-111">Связь</span><span class="sxs-lookup"><span data-stu-id="3cb32-111">Relationship</span></span> | <span data-ttu-id="3cb32-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb32-112">Type</span></span>   |<span data-ttu-id="3cb32-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb32-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cb32-114">категоряксис</span><span class="sxs-lookup"><span data-stu-id="3cb32-114">categoryAxis</span></span>|[<span data-ttu-id="3cb32-115">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="3cb32-115">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="3cb32-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb32-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="3cb32-118">сериесаксис</span><span class="sxs-lookup"><span data-stu-id="3cb32-118">seriesAxis</span></span>|[<span data-ttu-id="3cb32-119">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="3cb32-119">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="3cb32-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb32-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="3cb32-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="3cb32-122">valueAxis</span></span>|[<span data-ttu-id="3cb32-123">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="3cb32-123">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="3cb32-124">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="3cb32-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="3cb32-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb32-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb32-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cb32-126">JSON representation</span></span>

<span data-ttu-id="3cb32-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb32-127">Here is a JSON representation of the resource.</span></span>

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


