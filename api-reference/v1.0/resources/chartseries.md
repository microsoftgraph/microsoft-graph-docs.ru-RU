---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
ms.openlocfilehash: 60cd3e29f1b2c2f106fae0fdfb76b18657d68120
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314492"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="03e9d-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="03e9d-103">ChartSeries resource type</span></span>

<span data-ttu-id="03e9d-104">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="03e9d-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="03e9d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="03e9d-105">Methods</span></span>

| <span data-ttu-id="03e9d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="03e9d-106">Method</span></span>           | <span data-ttu-id="03e9d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03e9d-107">Return Type</span></span>    |<span data-ttu-id="03e9d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="03e9d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03e9d-109">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="03e9d-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="03e9d-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="03e9d-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="03e9d-111">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="03e9d-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="03e9d-112">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="03e9d-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="03e9d-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="03e9d-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="03e9d-114">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="03e9d-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="03e9d-115">Список точек</span><span class="sxs-lookup"><span data-stu-id="03e9d-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="03e9d-116">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="03e9d-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="03e9d-117">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="03e9d-117">Get a ChartPoints object collection.</span></span>|
|<span data-ttu-id="03e9d-118">[обновление](../api/chartseries-update.md).</span><span class="sxs-lookup"><span data-stu-id="03e9d-118">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="03e9d-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="03e9d-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="03e9d-120">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="03e9d-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="03e9d-121">List</span><span class="sxs-lookup"><span data-stu-id="03e9d-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="03e9d-122">[WorkbookChartSeries](chartseries.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="03e9d-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="03e9d-123">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="03e9d-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="03e9d-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="03e9d-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="03e9d-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="03e9d-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="03e9d-126">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="03e9d-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="03e9d-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="03e9d-127">Properties</span></span>
| <span data-ttu-id="03e9d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="03e9d-128">Property</span></span>     | <span data-ttu-id="03e9d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="03e9d-129">Type</span></span>   |<span data-ttu-id="03e9d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="03e9d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e9d-131">name</span><span class="sxs-lookup"><span data-stu-id="03e9d-131">name</span></span>|<span data-ttu-id="03e9d-132">строка</span><span class="sxs-lookup"><span data-stu-id="03e9d-132">string</span></span>|<span data-ttu-id="03e9d-133">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="03e9d-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03e9d-134">Связи</span><span class="sxs-lookup"><span data-stu-id="03e9d-134">Relationships</span></span>
| <span data-ttu-id="03e9d-135">Связь</span><span class="sxs-lookup"><span data-stu-id="03e9d-135">Relationship</span></span> | <span data-ttu-id="03e9d-136">Тип</span><span class="sxs-lookup"><span data-stu-id="03e9d-136">Type</span></span>   |<span data-ttu-id="03e9d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="03e9d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e9d-138">format</span><span class="sxs-lookup"><span data-stu-id="03e9d-138">format</span></span>|[<span data-ttu-id="03e9d-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="03e9d-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="03e9d-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03e9d-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="03e9d-142">points</span><span class="sxs-lookup"><span data-stu-id="03e9d-142">points</span></span>|<span data-ttu-id="03e9d-143">[WorkbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="03e9d-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="03e9d-p102">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03e9d-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03e9d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03e9d-146">JSON representation</span></span>

<span data-ttu-id="03e9d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03e9d-147">Here is a JSON representation of the resource.</span></span>

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