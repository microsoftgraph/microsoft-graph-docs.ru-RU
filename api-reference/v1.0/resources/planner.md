---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027717"
---
# <a name="planner-resource-type"></a><span data-ttu-id="27db4-105">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="27db4-105">planner resource type</span></span>

<span data-ttu-id="27db4-p102">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="27db4-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="27db4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="27db4-109">Methods</span></span>

| <span data-ttu-id="27db4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="27db4-110">Method</span></span>           | <span data-ttu-id="27db4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27db4-111">Return Type</span></span>    |<span data-ttu-id="27db4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="27db4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27db4-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="27db4-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="27db4-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="27db4-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="27db4-115">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="27db4-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="27db4-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="27db4-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="27db4-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="27db4-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="27db4-118">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="27db4-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="27db4-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="27db4-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="27db4-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="27db4-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="27db4-121">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="27db4-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27db4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="27db4-122">Relationships</span></span>
| <span data-ttu-id="27db4-123">Связь</span><span class="sxs-lookup"><span data-stu-id="27db4-123">Relationship</span></span> | <span data-ttu-id="27db4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="27db4-124">Type</span></span>   |<span data-ttu-id="27db4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="27db4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27db4-126">buckets</span><span class="sxs-lookup"><span data-stu-id="27db4-126">buckets</span></span>|<span data-ttu-id="27db4-127">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="27db4-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="27db4-p103">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="27db4-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="27db4-131">plans</span><span class="sxs-lookup"><span data-stu-id="27db4-131">plans</span></span>|<span data-ttu-id="27db4-132">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="27db4-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="27db4-p104">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="27db4-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="27db4-136">tasks</span><span class="sxs-lookup"><span data-stu-id="27db4-136">tasks</span></span>|<span data-ttu-id="27db4-137">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="27db4-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="27db4-p105">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="27db4-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27db4-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27db4-141">JSON representation</span></span>
<span data-ttu-id="27db4-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27db4-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="27db4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="27db4-143">Example</span></span>

<span data-ttu-id="27db4-144">**Планировщик работы** ресурсов доступна в корне диаграммы.</span><span class="sxs-lookup"><span data-stu-id="27db4-144">The **planner** resource is available at the root of the graph.</span></span>

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