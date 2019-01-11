---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f9bf959407a93c6d58d088833e5e3e437ef41125
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876253"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="42a35-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="42a35-103">ChartPoint resource type</span></span>

> <span data-ttu-id="42a35-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42a35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42a35-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42a35-106">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="42a35-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="42a35-107">Методы</span><span class="sxs-lookup"><span data-stu-id="42a35-107">Methods</span></span>

| <span data-ttu-id="42a35-108">Метод</span><span class="sxs-lookup"><span data-stu-id="42a35-108">Method</span></span>           | <span data-ttu-id="42a35-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42a35-109">Return Type</span></span>    |<span data-ttu-id="42a35-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42a35-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42a35-111">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="42a35-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="42a35-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="42a35-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="42a35-113">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="42a35-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="42a35-114">List</span><span class="sxs-lookup"><span data-stu-id="42a35-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="42a35-115">Коллекция объектов [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="42a35-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="42a35-116">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="42a35-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="42a35-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="42a35-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="42a35-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="42a35-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="42a35-119">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="42a35-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="42a35-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="42a35-120">Properties</span></span>
| <span data-ttu-id="42a35-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="42a35-121">Property</span></span>     | <span data-ttu-id="42a35-122">Тип</span><span class="sxs-lookup"><span data-stu-id="42a35-122">Type</span></span>   |<span data-ttu-id="42a35-123">Описание</span><span class="sxs-lookup"><span data-stu-id="42a35-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42a35-124">value</span><span class="sxs-lookup"><span data-stu-id="42a35-124">value</span></span>|<span data-ttu-id="42a35-125">object</span><span class="sxs-lookup"><span data-stu-id="42a35-125">object</span></span>|<span data-ttu-id="42a35-p102">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42a35-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42a35-128">Связи</span><span class="sxs-lookup"><span data-stu-id="42a35-128">Relationships</span></span>
| <span data-ttu-id="42a35-129">Связь</span><span class="sxs-lookup"><span data-stu-id="42a35-129">Relationship</span></span> | <span data-ttu-id="42a35-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42a35-130">Type</span></span>   |<span data-ttu-id="42a35-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42a35-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42a35-132">format</span><span class="sxs-lookup"><span data-stu-id="42a35-132">format</span></span>|[<span data-ttu-id="42a35-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="42a35-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="42a35-p103">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42a35-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42a35-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42a35-136">JSON representation</span></span>

<span data-ttu-id="42a35-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42a35-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
