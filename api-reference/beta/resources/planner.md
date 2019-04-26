---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2f1fb3b7058a87dd7b8390408590371cf1b0e9cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344629"
---
# <a name="planner-resource-type"></a><span data-ttu-id="ee73f-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="ee73f-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee73f-106">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="ee73f-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="ee73f-107">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="ee73f-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="ee73f-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="ee73f-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ee73f-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ee73f-109">Methods</span></span>

| <span data-ttu-id="ee73f-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ee73f-110">Method</span></span>           | <span data-ttu-id="ee73f-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee73f-111">Return Type</span></span>    |<span data-ttu-id="ee73f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ee73f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee73f-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ee73f-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="ee73f-114">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="ee73f-114">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="ee73f-115">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="ee73f-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="ee73f-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ee73f-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="ee73f-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ee73f-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="ee73f-118">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="ee73f-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="ee73f-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="ee73f-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="ee73f-120">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="ee73f-120">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="ee73f-121">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="ee73f-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee73f-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee73f-122">Properties</span></span>
| <span data-ttu-id="ee73f-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee73f-123">Property</span></span>     | <span data-ttu-id="ee73f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ee73f-124">Type</span></span>   |<span data-ttu-id="ee73f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ee73f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee73f-126">id</span><span class="sxs-lookup"><span data-stu-id="ee73f-126">id</span></span>|<span data-ttu-id="ee73f-127">String</span><span class="sxs-lookup"><span data-stu-id="ee73f-127">String</span></span>| <span data-ttu-id="ee73f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee73f-128">Read-only.</span></span> <span data-ttu-id="ee73f-129">Идентификатор ресурса **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="ee73f-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee73f-130">Связи</span><span class="sxs-lookup"><span data-stu-id="ee73f-130">Relationships</span></span>
| <span data-ttu-id="ee73f-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="ee73f-131">Relationship</span></span> | <span data-ttu-id="ee73f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ee73f-132">Type</span></span>   |<span data-ttu-id="ee73f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ee73f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee73f-134">buckets</span><span class="sxs-lookup"><span data-stu-id="ee73f-134">buckets</span></span>|<span data-ttu-id="ee73f-135">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="ee73f-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="ee73f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee73f-136">Read-only.</span></span> <span data-ttu-id="ee73f-137">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ee73f-137">Nullable.</span></span> <span data-ttu-id="ee73f-138">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="ee73f-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="ee73f-139">планирует</span><span class="sxs-lookup"><span data-stu-id="ee73f-139">plans</span></span>|<span data-ttu-id="ee73f-140">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ee73f-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ee73f-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee73f-141">Read-only.</span></span> <span data-ttu-id="ee73f-142">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ee73f-142">Nullable.</span></span> <span data-ttu-id="ee73f-143">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="ee73f-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="ee73f-144">tasks</span><span class="sxs-lookup"><span data-stu-id="ee73f-144">tasks</span></span>|<span data-ttu-id="ee73f-145">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ee73f-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ee73f-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee73f-146">Read-only.</span></span> <span data-ttu-id="ee73f-147">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ee73f-147">Nullable.</span></span> <span data-ttu-id="ee73f-148">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="ee73f-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee73f-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee73f-149">JSON representation</span></span>
<span data-ttu-id="ee73f-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee73f-150">Here is a JSON representation of the resource.</span></span>

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
