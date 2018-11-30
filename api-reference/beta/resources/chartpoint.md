---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
ms.openlocfilehash: 3d1bcc26fdc78bd7b844c870d40346a5f1f0496f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079518"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="d1e3d-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d1e3d-103">ChartPoint resource type</span></span>

> <span data-ttu-id="d1e3d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1e3d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1e3d-106">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d1e3d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d1e3d-107">Methods</span></span>

| <span data-ttu-id="d1e3d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d1e3d-108">Method</span></span>           | <span data-ttu-id="d1e3d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d1e3d-109">Return Type</span></span>    |<span data-ttu-id="d1e3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e3d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1e3d-111">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d1e3d-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="d1e3d-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d1e3d-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="d1e3d-113">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="d1e3d-114">List</span><span class="sxs-lookup"><span data-stu-id="d1e3d-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="d1e3d-115">Коллекция объектов [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="d1e3d-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="d1e3d-116">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="d1e3d-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="d1e3d-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="d1e3d-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d1e3d-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="d1e3d-119">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1e3d-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1e3d-120">Properties</span></span>
| <span data-ttu-id="d1e3d-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1e3d-121">Property</span></span>     | <span data-ttu-id="d1e3d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d1e3d-122">Type</span></span>   |<span data-ttu-id="d1e3d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e3d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1e3d-124">value</span><span class="sxs-lookup"><span data-stu-id="d1e3d-124">value</span></span>|<span data-ttu-id="d1e3d-125">object</span><span class="sxs-lookup"><span data-stu-id="d1e3d-125">object</span></span>|<span data-ttu-id="d1e3d-p102">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1e3d-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d1e3d-128">Relationships</span></span>
| <span data-ttu-id="d1e3d-129">Связь</span><span class="sxs-lookup"><span data-stu-id="d1e3d-129">Relationship</span></span> | <span data-ttu-id="d1e3d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1e3d-130">Type</span></span>   |<span data-ttu-id="d1e3d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e3d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1e3d-132">format</span><span class="sxs-lookup"><span data-stu-id="d1e3d-132">format</span></span>|[<span data-ttu-id="d1e3d-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="d1e3d-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="d1e3d-p103">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1e3d-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1e3d-136">JSON representation</span></span>

<span data-ttu-id="d1e3d-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1e3d-137">Here is a JSON representation of the resource.</span></span>

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