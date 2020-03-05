---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 45dc3ee05f5cee36ac1eecc99aff03f71b93c515
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521830"
---
# <a name="planner-resource-type"></a><span data-ttu-id="381a0-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="381a0-105">planner resource type</span></span>

<span data-ttu-id="381a0-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="381a0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="381a0-107">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="381a0-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="381a0-108">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="381a0-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="381a0-109">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="381a0-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="381a0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="381a0-110">Methods</span></span>

| <span data-ttu-id="381a0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="381a0-111">Method</span></span>           | <span data-ttu-id="381a0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="381a0-112">Return Type</span></span>    |<span data-ttu-id="381a0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="381a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="381a0-114">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="381a0-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="381a0-115">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="381a0-115">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="381a0-116">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="381a0-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="381a0-117">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="381a0-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="381a0-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="381a0-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="381a0-119">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="381a0-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="381a0-120">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="381a0-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="381a0-121">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="381a0-121">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="381a0-122">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="381a0-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="381a0-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="381a0-123">Properties</span></span>
| <span data-ttu-id="381a0-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="381a0-124">Property</span></span>     | <span data-ttu-id="381a0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="381a0-125">Type</span></span>   |<span data-ttu-id="381a0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="381a0-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="381a0-127">id</span><span class="sxs-lookup"><span data-stu-id="381a0-127">id</span></span>|<span data-ttu-id="381a0-128">String</span><span class="sxs-lookup"><span data-stu-id="381a0-128">String</span></span>| <span data-ttu-id="381a0-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="381a0-129">Read-only.</span></span> <span data-ttu-id="381a0-130">Идентификатор ресурса **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="381a0-130">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="381a0-131">Связи</span><span class="sxs-lookup"><span data-stu-id="381a0-131">Relationships</span></span>
| <span data-ttu-id="381a0-132">Связь</span><span class="sxs-lookup"><span data-stu-id="381a0-132">Relationship</span></span> | <span data-ttu-id="381a0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="381a0-133">Type</span></span>   |<span data-ttu-id="381a0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="381a0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="381a0-135">buckets</span><span class="sxs-lookup"><span data-stu-id="381a0-135">buckets</span></span>|<span data-ttu-id="381a0-136">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="381a0-136">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="381a0-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="381a0-137">Read-only.</span></span> <span data-ttu-id="381a0-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="381a0-138">Nullable.</span></span> <span data-ttu-id="381a0-139">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="381a0-139">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="381a0-140">планирует</span><span class="sxs-lookup"><span data-stu-id="381a0-140">plans</span></span>|<span data-ttu-id="381a0-141">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="381a0-141">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="381a0-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="381a0-142">Read-only.</span></span> <span data-ttu-id="381a0-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="381a0-143">Nullable.</span></span> <span data-ttu-id="381a0-144">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="381a0-144">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="381a0-145">tasks</span><span class="sxs-lookup"><span data-stu-id="381a0-145">tasks</span></span>|<span data-ttu-id="381a0-146">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="381a0-146">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="381a0-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="381a0-147">Read-only.</span></span> <span data-ttu-id="381a0-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="381a0-148">Nullable.</span></span> <span data-ttu-id="381a0-149">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="381a0-149">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="381a0-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="381a0-150">JSON representation</span></span>
<span data-ttu-id="381a0-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="381a0-151">Here is a JSON representation of the resource.</span></span>

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
