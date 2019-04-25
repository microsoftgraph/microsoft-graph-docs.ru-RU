---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579249"
---
# <a name="planner-resource-type"></a><span data-ttu-id="ae128-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="ae128-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae128-106">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="ae128-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="ae128-107">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="ae128-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="ae128-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="ae128-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ae128-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ae128-109">Methods</span></span>

| <span data-ttu-id="ae128-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ae128-110">Method</span></span>           | <span data-ttu-id="ae128-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae128-111">Return Type</span></span>    |<span data-ttu-id="ae128-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ae128-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae128-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ae128-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="ae128-114">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="ae128-114">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="ae128-115">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="ae128-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="ae128-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ae128-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="ae128-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ae128-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="ae128-118">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="ae128-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="ae128-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="ae128-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="ae128-120">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="ae128-120">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="ae128-121">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="ae128-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae128-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae128-122">Properties</span></span>
| <span data-ttu-id="ae128-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae128-123">Property</span></span>     | <span data-ttu-id="ae128-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ae128-124">Type</span></span>   |<span data-ttu-id="ae128-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ae128-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae128-126">id</span><span class="sxs-lookup"><span data-stu-id="ae128-126">id</span></span>|<span data-ttu-id="ae128-127">String</span><span class="sxs-lookup"><span data-stu-id="ae128-127">String</span></span>| <span data-ttu-id="ae128-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae128-128">Read-only.</span></span> <span data-ttu-id="ae128-129">Идентификатор ресурса **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="ae128-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae128-130">Связи</span><span class="sxs-lookup"><span data-stu-id="ae128-130">Relationships</span></span>
| <span data-ttu-id="ae128-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="ae128-131">Relationship</span></span> | <span data-ttu-id="ae128-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ae128-132">Type</span></span>   |<span data-ttu-id="ae128-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ae128-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae128-134">сегментов</span><span class="sxs-lookup"><span data-stu-id="ae128-134">buckets</span></span>|<span data-ttu-id="ae128-135">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="ae128-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="ae128-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae128-136">Read-only.</span></span> <span data-ttu-id="ae128-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ae128-137">Nullable.</span></span> <span data-ttu-id="ae128-138">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="ae128-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="ae128-139">планирует</span><span class="sxs-lookup"><span data-stu-id="ae128-139">plans</span></span>|<span data-ttu-id="ae128-140">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ae128-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ae128-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae128-141">Read-only.</span></span> <span data-ttu-id="ae128-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ae128-142">Nullable.</span></span> <span data-ttu-id="ae128-143">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="ae128-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="ae128-144">tasks</span><span class="sxs-lookup"><span data-stu-id="ae128-144">tasks</span></span>|<span data-ttu-id="ae128-145">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ae128-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ae128-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae128-146">Read-only.</span></span> <span data-ttu-id="ae128-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ae128-147">Nullable.</span></span> <span data-ttu-id="ae128-148">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="ae128-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae128-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae128-149">JSON representation</span></span>
<span data-ttu-id="ae128-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae128-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
