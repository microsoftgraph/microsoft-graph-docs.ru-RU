---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5606516092633ff14d23947f73626adc6d83c2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460998"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="27542-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="27542-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27542-104">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="27542-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="27542-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27542-105">Methods</span></span>

| <span data-ttu-id="27542-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27542-106">Method</span></span>           | <span data-ttu-id="27542-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27542-107">Return Type</span></span>    |<span data-ttu-id="27542-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27542-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27542-109">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="27542-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="27542-110">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="27542-110">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="27542-111">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="27542-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="27542-112">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="27542-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="27542-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="27542-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="27542-114">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="27542-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="27542-115">Список точек</span><span class="sxs-lookup"><span data-stu-id="27542-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="27542-116">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="27542-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="27542-117">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="27542-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="27542-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="27542-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="27542-119">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="27542-119">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="27542-120">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="27542-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="27542-121">Список</span><span class="sxs-lookup"><span data-stu-id="27542-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="27542-122">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="27542-122">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="27542-123">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="27542-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="27542-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="27542-124">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="27542-125">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="27542-125">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="27542-126">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="27542-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="27542-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="27542-127">Properties</span></span>
| <span data-ttu-id="27542-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="27542-128">Property</span></span>     | <span data-ttu-id="27542-129">Тип</span><span class="sxs-lookup"><span data-stu-id="27542-129">Type</span></span>   |<span data-ttu-id="27542-130">Описание</span><span class="sxs-lookup"><span data-stu-id="27542-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27542-131">name</span><span class="sxs-lookup"><span data-stu-id="27542-131">name</span></span>|<span data-ttu-id="27542-132">string</span><span class="sxs-lookup"><span data-stu-id="27542-132">string</span></span>|<span data-ttu-id="27542-133">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="27542-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27542-134">Связи</span><span class="sxs-lookup"><span data-stu-id="27542-134">Relationships</span></span>
| <span data-ttu-id="27542-135">Отношение</span><span class="sxs-lookup"><span data-stu-id="27542-135">Relationship</span></span> | <span data-ttu-id="27542-136">Тип</span><span class="sxs-lookup"><span data-stu-id="27542-136">Type</span></span>   |<span data-ttu-id="27542-137">Описание</span><span class="sxs-lookup"><span data-stu-id="27542-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27542-138">format</span><span class="sxs-lookup"><span data-stu-id="27542-138">format</span></span>|[<span data-ttu-id="27542-139">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="27542-139">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="27542-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27542-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="27542-142">points</span><span class="sxs-lookup"><span data-stu-id="27542-142">points</span></span>|<span data-ttu-id="27542-143">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="27542-143">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="27542-p102">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27542-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27542-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27542-146">JSON representation</span></span>

<span data-ttu-id="27542-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27542-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
