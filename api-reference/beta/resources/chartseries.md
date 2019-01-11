---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6742c30eca55426e54290ae689bfabd8e14ce70f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842632"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="71985-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="71985-103">ChartSeries resource type</span></span>

> <span data-ttu-id="71985-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71985-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71985-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71985-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71985-106">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="71985-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="71985-107">Методы</span><span class="sxs-lookup"><span data-stu-id="71985-107">Methods</span></span>

| <span data-ttu-id="71985-108">Метод</span><span class="sxs-lookup"><span data-stu-id="71985-108">Method</span></span>           | <span data-ttu-id="71985-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71985-109">Return Type</span></span>    |<span data-ttu-id="71985-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71985-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71985-111">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="71985-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="71985-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="71985-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="71985-113">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="71985-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="71985-114">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="71985-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="71985-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="71985-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="71985-116">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="71985-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="71985-117">Список точек</span><span class="sxs-lookup"><span data-stu-id="71985-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="71985-118">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="71985-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="71985-119">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="71985-119">Get a ChartPoints object collection.</span></span>|
|<span data-ttu-id="71985-120">[обновление](../api/chartseries-update.md).</span><span class="sxs-lookup"><span data-stu-id="71985-120">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="71985-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="71985-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="71985-122">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="71985-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="71985-123">List</span><span class="sxs-lookup"><span data-stu-id="71985-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="71985-124">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="71985-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="71985-125">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="71985-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="71985-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="71985-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="71985-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="71985-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="71985-128">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="71985-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="71985-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="71985-129">Properties</span></span>
| <span data-ttu-id="71985-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71985-130">Property</span></span>     | <span data-ttu-id="71985-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71985-131">Type</span></span>   |<span data-ttu-id="71985-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71985-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71985-133">name</span><span class="sxs-lookup"><span data-stu-id="71985-133">name</span></span>|<span data-ttu-id="71985-134">строка</span><span class="sxs-lookup"><span data-stu-id="71985-134">string</span></span>|<span data-ttu-id="71985-135">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="71985-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71985-136">Связи</span><span class="sxs-lookup"><span data-stu-id="71985-136">Relationships</span></span>
| <span data-ttu-id="71985-137">Связь</span><span class="sxs-lookup"><span data-stu-id="71985-137">Relationship</span></span> | <span data-ttu-id="71985-138">Тип</span><span class="sxs-lookup"><span data-stu-id="71985-138">Type</span></span>   |<span data-ttu-id="71985-139">Описание</span><span class="sxs-lookup"><span data-stu-id="71985-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71985-140">format</span><span class="sxs-lookup"><span data-stu-id="71985-140">format</span></span>|[<span data-ttu-id="71985-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="71985-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="71985-p102">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71985-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="71985-144">points</span><span class="sxs-lookup"><span data-stu-id="71985-144">points</span></span>|<span data-ttu-id="71985-145">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="71985-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="71985-p103">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71985-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71985-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71985-148">JSON representation</span></span>

<span data-ttu-id="71985-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71985-149">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
