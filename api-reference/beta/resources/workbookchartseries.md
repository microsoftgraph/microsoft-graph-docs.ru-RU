---
title: Тип ресурса Воркбукчартсериес
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2f93eb5ccf8b3acda9113312f4dbbb9063bdfcef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519276"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="c3aac-103">Тип ресурса Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="c3aac-103">workbookChartSeries resource type</span></span>

<span data-ttu-id="c3aac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3aac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3aac-105">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="c3aac-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c3aac-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c3aac-106">Methods</span></span>

| <span data-ttu-id="c3aac-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c3aac-107">Method</span></span>           | <span data-ttu-id="c3aac-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3aac-108">Return Type</span></span>    |<span data-ttu-id="c3aac-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c3aac-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3aac-110">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c3aac-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="c3aac-111">воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="c3aac-111">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c3aac-112">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="c3aac-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="c3aac-113">Создание ChartPoint</span><span class="sxs-lookup"><span data-stu-id="c3aac-113">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="c3aac-114">chartPoints</span><span class="sxs-lookup"><span data-stu-id="c3aac-114">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="c3aac-115">Создание нового chartPoint путем публикации в коллекции Points.</span><span class="sxs-lookup"><span data-stu-id="c3aac-115">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="c3aac-116">Список точек</span><span class="sxs-lookup"><span data-stu-id="c3aac-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="c3aac-117">Коллекция [воркбукчартпоинтс](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c3aac-117">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="c3aac-118">Получение коллекции объектов chartPoints.</span><span class="sxs-lookup"><span data-stu-id="c3aac-118">Get a chartPoints object collection.</span></span>|
|<span data-ttu-id="c3aac-119">[обновление](../api/chartseries-update.md).</span><span class="sxs-lookup"><span data-stu-id="c3aac-119">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="c3aac-120">воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="c3aac-120">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c3aac-121">Обновление объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="c3aac-121">Update chartSeries object.</span></span> |
|[<span data-ttu-id="c3aac-122">List</span><span class="sxs-lookup"><span data-stu-id="c3aac-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="c3aac-123">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="c3aac-123">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="c3aac-124">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="c3aac-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="c3aac-125">итемат</span><span class="sxs-lookup"><span data-stu-id="c3aac-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="c3aac-126">воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="c3aac-126">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="c3aac-127">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="c3aac-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="c3aac-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3aac-128">Properties</span></span>
| <span data-ttu-id="c3aac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3aac-129">Property</span></span>     | <span data-ttu-id="c3aac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3aac-130">Type</span></span>   |<span data-ttu-id="c3aac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3aac-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3aac-132">name</span><span class="sxs-lookup"><span data-stu-id="c3aac-132">name</span></span>|<span data-ttu-id="c3aac-133">string</span><span class="sxs-lookup"><span data-stu-id="c3aac-133">string</span></span>|<span data-ttu-id="c3aac-134">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="c3aac-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3aac-135">Связи</span><span class="sxs-lookup"><span data-stu-id="c3aac-135">Relationships</span></span>
| <span data-ttu-id="c3aac-136">Связь</span><span class="sxs-lookup"><span data-stu-id="c3aac-136">Relationship</span></span> | <span data-ttu-id="c3aac-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c3aac-137">Type</span></span>   |<span data-ttu-id="c3aac-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c3aac-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3aac-139">format</span><span class="sxs-lookup"><span data-stu-id="c3aac-139">format</span></span>|[<span data-ttu-id="c3aac-140">воркбукчартсериесформат</span><span class="sxs-lookup"><span data-stu-id="c3aac-140">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="c3aac-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3aac-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="c3aac-143">points</span><span class="sxs-lookup"><span data-stu-id="c3aac-143">points</span></span>|<span data-ttu-id="c3aac-144">Коллекция [воркбукчартпоинт](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c3aac-144">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="c3aac-145">Представляет коллекцию всех точек в ряду.</span><span class="sxs-lookup"><span data-stu-id="c3aac-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="c3aac-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3aac-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3aac-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3aac-147">JSON representation</span></span>

<span data-ttu-id="c3aac-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3aac-148">Here is a JSON representation of the resource.</span></span>

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
