---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ef94a7507558279e5295239588e2a8eda512882
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009134"
---
# <a name="planner-resource-type"></a><span data-ttu-id="39816-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="39816-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39816-106">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="39816-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="39816-107">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="39816-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="39816-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="39816-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="39816-109">Методы</span><span class="sxs-lookup"><span data-stu-id="39816-109">Methods</span></span>

| <span data-ttu-id="39816-110">Метод</span><span class="sxs-lookup"><span data-stu-id="39816-110">Method</span></span>           | <span data-ttu-id="39816-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="39816-111">Return Type</span></span>    |<span data-ttu-id="39816-112">Описание</span><span class="sxs-lookup"><span data-stu-id="39816-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39816-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="39816-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="39816-114">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="39816-114">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="39816-115">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="39816-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="39816-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="39816-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="39816-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="39816-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="39816-118">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="39816-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="39816-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="39816-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="39816-120">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="39816-120">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="39816-121">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="39816-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="39816-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="39816-122">Properties</span></span>
| <span data-ttu-id="39816-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="39816-123">Property</span></span>     | <span data-ttu-id="39816-124">Тип</span><span class="sxs-lookup"><span data-stu-id="39816-124">Type</span></span>   |<span data-ttu-id="39816-125">Описание</span><span class="sxs-lookup"><span data-stu-id="39816-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39816-126">id</span><span class="sxs-lookup"><span data-stu-id="39816-126">id</span></span>|<span data-ttu-id="39816-127">String</span><span class="sxs-lookup"><span data-stu-id="39816-127">String</span></span>| <span data-ttu-id="39816-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39816-128">Read-only.</span></span> <span data-ttu-id="39816-129">Идентификатор ресурса **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="39816-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39816-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="39816-130">Relationships</span></span>
| <span data-ttu-id="39816-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="39816-131">Relationship</span></span> | <span data-ttu-id="39816-132">Тип</span><span class="sxs-lookup"><span data-stu-id="39816-132">Type</span></span>   |<span data-ttu-id="39816-133">Описание</span><span class="sxs-lookup"><span data-stu-id="39816-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39816-134">buckets</span><span class="sxs-lookup"><span data-stu-id="39816-134">buckets</span></span>|<span data-ttu-id="39816-135">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="39816-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="39816-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39816-136">Read-only.</span></span> <span data-ttu-id="39816-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="39816-137">Nullable.</span></span> <span data-ttu-id="39816-138">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="39816-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="39816-139">планирует</span><span class="sxs-lookup"><span data-stu-id="39816-139">plans</span></span>|<span data-ttu-id="39816-140">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="39816-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="39816-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39816-141">Read-only.</span></span> <span data-ttu-id="39816-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="39816-142">Nullable.</span></span> <span data-ttu-id="39816-143">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="39816-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="39816-144">tasks</span><span class="sxs-lookup"><span data-stu-id="39816-144">tasks</span></span>|<span data-ttu-id="39816-145">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="39816-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="39816-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39816-146">Read-only.</span></span> <span data-ttu-id="39816-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="39816-147">Nullable.</span></span> <span data-ttu-id="39816-148">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="39816-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39816-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39816-149">JSON representation</span></span>
<span data-ttu-id="39816-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39816-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
