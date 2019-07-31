---
title: Тип ресурса Воркбукчартсериес
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c7f7c8108ac17e6705b8bf5f69b0e87f0dc96b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007251"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="3013b-103">Тип ресурса Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="3013b-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3013b-104">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3013b-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="3013b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3013b-105">Methods</span></span>

| <span data-ttu-id="3013b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3013b-106">Method</span></span>           | <span data-ttu-id="3013b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3013b-107">Return Type</span></span>    |<span data-ttu-id="3013b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3013b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3013b-109">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="3013b-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="3013b-110">Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="3013b-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="3013b-111">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="3013b-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="3013b-112">Создание ChartPoint</span><span class="sxs-lookup"><span data-stu-id="3013b-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="3013b-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="3013b-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="3013b-114">Создание нового chartPoint путем публикации в коллекции Points.</span><span class="sxs-lookup"><span data-stu-id="3013b-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="3013b-115">Список точек</span><span class="sxs-lookup"><span data-stu-id="3013b-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="3013b-116">Коллекция [воркбукчартпоинтс](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="3013b-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="3013b-117">Получение коллекции объектов chartPoints.</span><span class="sxs-lookup"><span data-stu-id="3013b-117">Get a chartPoints object collection.</span></span>|
|<span data-ttu-id="3013b-118">[обновление](../api/chartseries-update.md);</span><span class="sxs-lookup"><span data-stu-id="3013b-118">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="3013b-119">Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="3013b-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="3013b-120">Обновление объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="3013b-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="3013b-121">List</span><span class="sxs-lookup"><span data-stu-id="3013b-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="3013b-122">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="3013b-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="3013b-123">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="3013b-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="3013b-124">Итемат</span><span class="sxs-lookup"><span data-stu-id="3013b-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="3013b-125">Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="3013b-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="3013b-126">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="3013b-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="3013b-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="3013b-127">Properties</span></span>
| <span data-ttu-id="3013b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3013b-128">Property</span></span>     | <span data-ttu-id="3013b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3013b-129">Type</span></span>   |<span data-ttu-id="3013b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3013b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3013b-131">name</span><span class="sxs-lookup"><span data-stu-id="3013b-131">name</span></span>|<span data-ttu-id="3013b-132">string</span><span class="sxs-lookup"><span data-stu-id="3013b-132">string</span></span>|<span data-ttu-id="3013b-133">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3013b-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3013b-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="3013b-134">Relationships</span></span>
| <span data-ttu-id="3013b-135">Отношение</span><span class="sxs-lookup"><span data-stu-id="3013b-135">Relationship</span></span> | <span data-ttu-id="3013b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="3013b-136">Type</span></span>   |<span data-ttu-id="3013b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3013b-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3013b-138">format</span><span class="sxs-lookup"><span data-stu-id="3013b-138">format</span></span>|[<span data-ttu-id="3013b-139">Воркбукчартсериесформат</span><span class="sxs-lookup"><span data-stu-id="3013b-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="3013b-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3013b-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="3013b-142">points</span><span class="sxs-lookup"><span data-stu-id="3013b-142">points</span></span>|<span data-ttu-id="3013b-143">Коллекция [воркбукчартпоинт](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="3013b-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="3013b-144">Представляет коллекцию всех точек в ряду.</span><span class="sxs-lookup"><span data-stu-id="3013b-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="3013b-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3013b-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3013b-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3013b-146">JSON representation</span></span>

<span data-ttu-id="3013b-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3013b-147">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
