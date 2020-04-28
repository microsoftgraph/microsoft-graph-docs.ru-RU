---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 89d9a45f0f9e992ac8a93cde6114fc8c9f073359
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519388"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="1be1f-103">Тип ресурса Воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="1be1f-103">workbookChartAxes resource type</span></span>

<span data-ttu-id="1be1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be1f-105">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1be1f-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="1be1f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1be1f-106">Methods</span></span>
<span data-ttu-id="1be1f-107">Нет</span><span class="sxs-lookup"><span data-stu-id="1be1f-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="1be1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1be1f-108">Properties</span></span>
<span data-ttu-id="1be1f-109">Нет</span><span class="sxs-lookup"><span data-stu-id="1be1f-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1be1f-110">Связи</span><span class="sxs-lookup"><span data-stu-id="1be1f-110">Relationships</span></span>
| <span data-ttu-id="1be1f-111">Связь</span><span class="sxs-lookup"><span data-stu-id="1be1f-111">Relationship</span></span> | <span data-ttu-id="1be1f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="1be1f-112">Type</span></span>   |<span data-ttu-id="1be1f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1be1f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1be1f-114">категоряксис</span><span class="sxs-lookup"><span data-stu-id="1be1f-114">categoryAxis</span></span>|[<span data-ttu-id="1be1f-115">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1be1f-115">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1be1f-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1be1f-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="1be1f-118">сериесаксис</span><span class="sxs-lookup"><span data-stu-id="1be1f-118">seriesAxis</span></span>|[<span data-ttu-id="1be1f-119">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1be1f-119">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1be1f-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1be1f-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="1be1f-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="1be1f-122">valueAxis</span></span>|[<span data-ttu-id="1be1f-123">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1be1f-123">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1be1f-124">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="1be1f-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="1be1f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1be1f-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1be1f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1be1f-126">JSON representation</span></span>

<span data-ttu-id="1be1f-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1be1f-127">Here is a JSON representation of the resource.</span></span>

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
