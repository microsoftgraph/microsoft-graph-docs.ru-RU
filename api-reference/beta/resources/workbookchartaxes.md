---
title: Тип ресурса Воркбукчартаксес
description: Представляет оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15e63af1e7b648288dba813790302f1dee6536ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348946"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="1ca10-103">Тип ресурса Воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="1ca10-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca10-104">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1ca10-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="1ca10-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1ca10-105">Methods</span></span>
<span data-ttu-id="1ca10-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="1ca10-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1ca10-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ca10-107">Properties</span></span>
<span data-ttu-id="1ca10-108">Нет</span><span class="sxs-lookup"><span data-stu-id="1ca10-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1ca10-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ca10-109">Relationships</span></span>
| <span data-ttu-id="1ca10-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="1ca10-110">Relationship</span></span> | <span data-ttu-id="1ca10-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1ca10-111">Type</span></span>   |<span data-ttu-id="1ca10-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca10-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ca10-113">Категоряксис</span><span class="sxs-lookup"><span data-stu-id="1ca10-113">categoryAxis</span></span>|[<span data-ttu-id="1ca10-114">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1ca10-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1ca10-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ca10-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="1ca10-117">Сериесаксис</span><span class="sxs-lookup"><span data-stu-id="1ca10-117">seriesAxis</span></span>|[<span data-ttu-id="1ca10-118">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1ca10-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1ca10-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ca10-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="1ca10-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="1ca10-121">valueAxis</span></span>|[<span data-ttu-id="1ca10-122">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1ca10-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="1ca10-123">Представляет ось значений для оси.</span><span class="sxs-lookup"><span data-stu-id="1ca10-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="1ca10-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ca10-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ca10-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ca10-125">JSON representation</span></span>

<span data-ttu-id="1ca10-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ca10-126">Here is a JSON representation of the resource.</span></span>

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
