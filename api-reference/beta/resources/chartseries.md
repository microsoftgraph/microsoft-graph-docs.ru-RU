---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eccd0d970ffeff7b41ceb0f9af810bb7a420d663
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570661"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="32071-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="32071-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32071-104">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="32071-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="32071-105">Методы</span><span class="sxs-lookup"><span data-stu-id="32071-105">Methods</span></span>

| <span data-ttu-id="32071-106">Метод</span><span class="sxs-lookup"><span data-stu-id="32071-106">Method</span></span>           | <span data-ttu-id="32071-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32071-107">Return Type</span></span>    |<span data-ttu-id="32071-108">Описание</span><span class="sxs-lookup"><span data-stu-id="32071-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32071-109">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="32071-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="32071-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="32071-110">workbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="32071-111">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="32071-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="32071-112">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="32071-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="32071-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="32071-113">chartPoints</span></span>](chartpoint.md)| <span data-ttu-id="32071-114">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="32071-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="32071-115">Список точек</span><span class="sxs-lookup"><span data-stu-id="32071-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="32071-116">[chartPoints](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="32071-116">[chartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="32071-117">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="32071-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="32071-118">Update</span><span class="sxs-lookup"><span data-stu-id="32071-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="32071-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="32071-119">workbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="32071-120">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="32071-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="32071-121">List</span><span class="sxs-lookup"><span data-stu-id="32071-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="32071-122">[workbookChartSeries](chartseries.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="32071-122">[workbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="32071-123">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="32071-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="32071-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="32071-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="32071-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="32071-125">workbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="32071-126">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="32071-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="32071-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="32071-127">Properties</span></span>
| <span data-ttu-id="32071-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="32071-128">Property</span></span>     | <span data-ttu-id="32071-129">Тип</span><span class="sxs-lookup"><span data-stu-id="32071-129">Type</span></span>   |<span data-ttu-id="32071-130">Описание</span><span class="sxs-lookup"><span data-stu-id="32071-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32071-131">name</span><span class="sxs-lookup"><span data-stu-id="32071-131">name</span></span>|<span data-ttu-id="32071-132">строка</span><span class="sxs-lookup"><span data-stu-id="32071-132">string</span></span>|<span data-ttu-id="32071-133">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="32071-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32071-134">Связи</span><span class="sxs-lookup"><span data-stu-id="32071-134">Relationships</span></span>
| <span data-ttu-id="32071-135">Связь</span><span class="sxs-lookup"><span data-stu-id="32071-135">Relationship</span></span> | <span data-ttu-id="32071-136">Тип</span><span class="sxs-lookup"><span data-stu-id="32071-136">Type</span></span>   |<span data-ttu-id="32071-137">Описание</span><span class="sxs-lookup"><span data-stu-id="32071-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32071-138">format</span><span class="sxs-lookup"><span data-stu-id="32071-138">format</span></span>|[<span data-ttu-id="32071-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="32071-139">workbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="32071-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32071-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="32071-142">points</span><span class="sxs-lookup"><span data-stu-id="32071-142">points</span></span>|<span data-ttu-id="32071-143">[workbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="32071-143">[workbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="32071-p102">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32071-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32071-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32071-146">JSON representation</span></span>

<span data-ttu-id="32071-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32071-147">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
