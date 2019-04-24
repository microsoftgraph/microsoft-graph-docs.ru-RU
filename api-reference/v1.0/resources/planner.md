---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462279"
---
# <a name="planner-resource-type"></a><span data-ttu-id="bb310-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="bb310-105">planner resource type</span></span>

<span data-ttu-id="bb310-106">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="bb310-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="bb310-107">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="bb310-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="bb310-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="bb310-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="bb310-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bb310-109">Methods</span></span>

| <span data-ttu-id="bb310-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bb310-110">Method</span></span>           | <span data-ttu-id="bb310-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb310-111">Return Type</span></span>    |<span data-ttu-id="bb310-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bb310-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb310-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="bb310-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="bb310-114">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="bb310-114">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="bb310-115">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="bb310-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="bb310-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bb310-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="bb310-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bb310-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="bb310-118">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="bb310-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="bb310-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="bb310-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="bb310-120">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="bb310-120">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="bb310-121">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="bb310-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb310-122">Связи</span><span class="sxs-lookup"><span data-stu-id="bb310-122">Relationships</span></span>
| <span data-ttu-id="bb310-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="bb310-123">Relationship</span></span> | <span data-ttu-id="bb310-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bb310-124">Type</span></span>   |<span data-ttu-id="bb310-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bb310-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb310-126">сегментов</span><span class="sxs-lookup"><span data-stu-id="bb310-126">buckets</span></span>|<span data-ttu-id="bb310-127">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="bb310-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="bb310-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb310-128">Read-only.</span></span> <span data-ttu-id="bb310-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bb310-129">Nullable.</span></span> <span data-ttu-id="bb310-130">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="bb310-130">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="bb310-131">планирует</span><span class="sxs-lookup"><span data-stu-id="bb310-131">plans</span></span>|<span data-ttu-id="bb310-132">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="bb310-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bb310-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb310-133">Read-only.</span></span> <span data-ttu-id="bb310-134">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bb310-134">Nullable.</span></span> <span data-ttu-id="bb310-135">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="bb310-135">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="bb310-136">tasks</span><span class="sxs-lookup"><span data-stu-id="bb310-136">tasks</span></span>|<span data-ttu-id="bb310-137">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="bb310-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bb310-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb310-138">Read-only.</span></span> <span data-ttu-id="bb310-139">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bb310-139">Nullable.</span></span> <span data-ttu-id="bb310-140">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="bb310-140">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb310-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb310-141">JSON representation</span></span>
<span data-ttu-id="bb310-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb310-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="bb310-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bb310-143">Example</span></span>

<span data-ttu-id="bb310-144">Ресурс **планировщика** доступен в корневом каталоге диаграммы.</span><span class="sxs-lookup"><span data-stu-id="bb310-144">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
