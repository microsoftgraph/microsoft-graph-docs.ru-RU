---
title: Тип ресурса ChartSeries
description: Представляет ряд в диаграмме.
author: lumine2008
ms.openlocfilehash: 443b6b3dfea54b59ff92babc2776d9624bd28b20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325286"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="744a0-103">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="744a0-103">ChartSeries resource type</span></span>

> <span data-ttu-id="744a0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="744a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="744a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="744a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="744a0-106">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="744a0-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="744a0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="744a0-107">Methods</span></span>

| <span data-ttu-id="744a0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="744a0-108">Method</span></span>           | <span data-ttu-id="744a0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="744a0-109">Return Type</span></span>    |<span data-ttu-id="744a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="744a0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="744a0-111">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="744a0-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="744a0-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="744a0-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="744a0-113">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="744a0-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="744a0-114">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="744a0-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="744a0-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="744a0-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="744a0-116">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="744a0-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="744a0-117">Список точек</span><span class="sxs-lookup"><span data-stu-id="744a0-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="744a0-118">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="744a0-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="744a0-119">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="744a0-119">Get a ChartPoints object collection.</span></span>|
|<span data-ttu-id="744a0-120">[обновление](../api/chartseries-update.md).</span><span class="sxs-lookup"><span data-stu-id="744a0-120">[Update](../api/chartseries-update.md)</span></span> | [<span data-ttu-id="744a0-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="744a0-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="744a0-122">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="744a0-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="744a0-123">List</span><span class="sxs-lookup"><span data-stu-id="744a0-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="744a0-124">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="744a0-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="744a0-125">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="744a0-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="744a0-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="744a0-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="744a0-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="744a0-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="744a0-128">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="744a0-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="744a0-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="744a0-129">Properties</span></span>
| <span data-ttu-id="744a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="744a0-130">Property</span></span>     | <span data-ttu-id="744a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="744a0-131">Type</span></span>   |<span data-ttu-id="744a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="744a0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="744a0-133">name</span><span class="sxs-lookup"><span data-stu-id="744a0-133">name</span></span>|<span data-ttu-id="744a0-134">строка</span><span class="sxs-lookup"><span data-stu-id="744a0-134">string</span></span>|<span data-ttu-id="744a0-135">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="744a0-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="744a0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="744a0-136">Relationships</span></span>
| <span data-ttu-id="744a0-137">Связь</span><span class="sxs-lookup"><span data-stu-id="744a0-137">Relationship</span></span> | <span data-ttu-id="744a0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="744a0-138">Type</span></span>   |<span data-ttu-id="744a0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="744a0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="744a0-140">format</span><span class="sxs-lookup"><span data-stu-id="744a0-140">format</span></span>|[<span data-ttu-id="744a0-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="744a0-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="744a0-p102">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="744a0-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="744a0-144">points</span><span class="sxs-lookup"><span data-stu-id="744a0-144">points</span></span>|<span data-ttu-id="744a0-145">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="744a0-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="744a0-p103">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="744a0-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="744a0-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="744a0-148">JSON representation</span></span>

<span data-ttu-id="744a0-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="744a0-149">Here is a JSON representation of the resource.</span></span>

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