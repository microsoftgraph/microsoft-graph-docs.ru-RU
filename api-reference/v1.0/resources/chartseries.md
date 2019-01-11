---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a3a19793629a5e100830565e224541930e2180de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834897"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="7f4f7-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="7f4f7-103">ChartSeries resource type</span></span>

<span data-ttu-id="7f4f7-104">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7f4f7-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7f4f7-105">Methods</span></span>

| <span data-ttu-id="7f4f7-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7f4f7-106">Method</span></span>           | <span data-ttu-id="7f4f7-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f4f7-107">Return Type</span></span>    |<span data-ttu-id="7f4f7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4f7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f4f7-109">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="7f4f7-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="7f4f7-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="7f4f7-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="7f4f7-111">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="7f4f7-112">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="7f4f7-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="7f4f7-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="7f4f7-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="7f4f7-114">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="7f4f7-115">Список точек</span><span class="sxs-lookup"><span data-stu-id="7f4f7-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="7f4f7-116">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="7f4f7-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="7f4f7-117">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-117">Get a ChartPoints object collection.</span></span>|
|<span data-ttu-id="7f4f7-118">[обновление](../api/chartseries-update.md).</span><span class="sxs-lookup"><span data-stu-id="7f4f7-118">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="7f4f7-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="7f4f7-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="7f4f7-120">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="7f4f7-121">List</span><span class="sxs-lookup"><span data-stu-id="7f4f7-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="7f4f7-122">[WorkbookChartSeries](chartseries.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7f4f7-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="7f4f7-123">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="7f4f7-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="7f4f7-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="7f4f7-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="7f4f7-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="7f4f7-126">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="7f4f7-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f4f7-127">Properties</span></span>
| <span data-ttu-id="7f4f7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f4f7-128">Property</span></span>     | <span data-ttu-id="7f4f7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7f4f7-129">Type</span></span>   |<span data-ttu-id="7f4f7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4f7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4f7-131">name</span><span class="sxs-lookup"><span data-stu-id="7f4f7-131">name</span></span>|<span data-ttu-id="7f4f7-132">строка</span><span class="sxs-lookup"><span data-stu-id="7f4f7-132">string</span></span>|<span data-ttu-id="7f4f7-133">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f4f7-134">Связи</span><span class="sxs-lookup"><span data-stu-id="7f4f7-134">Relationships</span></span>
| <span data-ttu-id="7f4f7-135">Связь</span><span class="sxs-lookup"><span data-stu-id="7f4f7-135">Relationship</span></span> | <span data-ttu-id="7f4f7-136">Тип</span><span class="sxs-lookup"><span data-stu-id="7f4f7-136">Type</span></span>   |<span data-ttu-id="7f4f7-137">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4f7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4f7-138">format</span><span class="sxs-lookup"><span data-stu-id="7f4f7-138">format</span></span>|[<span data-ttu-id="7f4f7-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="7f4f7-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="7f4f7-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="7f4f7-142">points</span><span class="sxs-lookup"><span data-stu-id="7f4f7-142">points</span></span>|<span data-ttu-id="7f4f7-143">[WorkbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7f4f7-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="7f4f7-p102">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f4f7-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f4f7-146">JSON representation</span></span>

<span data-ttu-id="7f4f7-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f4f7-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
