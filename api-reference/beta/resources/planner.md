---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
ms.openlocfilehash: c076eda1660cef9e31f584e5fe439f916eba81d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082664"
---
# <a name="planner-resource-type"></a><span data-ttu-id="be0ee-105">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="be0ee-105">planner resource type</span></span>

> <span data-ttu-id="be0ee-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be0ee-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be0ee-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be0ee-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be0ee-p103">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="be0ee-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="be0ee-111">Методы</span><span class="sxs-lookup"><span data-stu-id="be0ee-111">Methods</span></span>

| <span data-ttu-id="be0ee-112">Метод</span><span class="sxs-lookup"><span data-stu-id="be0ee-112">Method</span></span>           | <span data-ttu-id="be0ee-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be0ee-113">Return Type</span></span>    |<span data-ttu-id="be0ee-114">Описание</span><span class="sxs-lookup"><span data-stu-id="be0ee-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be0ee-115">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="be0ee-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="be0ee-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="be0ee-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="be0ee-117">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="be0ee-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="be0ee-118">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="be0ee-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="be0ee-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="be0ee-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="be0ee-120">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="be0ee-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="be0ee-121">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="be0ee-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="be0ee-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="be0ee-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="be0ee-123">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="be0ee-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="be0ee-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="be0ee-124">Properties</span></span>
| <span data-ttu-id="be0ee-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="be0ee-125">Property</span></span>     | <span data-ttu-id="be0ee-126">Тип</span><span class="sxs-lookup"><span data-stu-id="be0ee-126">Type</span></span>   |<span data-ttu-id="be0ee-127">Описание</span><span class="sxs-lookup"><span data-stu-id="be0ee-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be0ee-128">id</span><span class="sxs-lookup"><span data-stu-id="be0ee-128">id</span></span>|<span data-ttu-id="be0ee-129">String</span><span class="sxs-lookup"><span data-stu-id="be0ee-129">String</span></span>| <span data-ttu-id="be0ee-p104">Только для чтения. Идентификатор ресурса **planner**.</span><span class="sxs-lookup"><span data-stu-id="be0ee-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be0ee-132">Связи</span><span class="sxs-lookup"><span data-stu-id="be0ee-132">Relationships</span></span>
| <span data-ttu-id="be0ee-133">Связь</span><span class="sxs-lookup"><span data-stu-id="be0ee-133">Relationship</span></span> | <span data-ttu-id="be0ee-134">Тип</span><span class="sxs-lookup"><span data-stu-id="be0ee-134">Type</span></span>   |<span data-ttu-id="be0ee-135">Описание</span><span class="sxs-lookup"><span data-stu-id="be0ee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be0ee-136">buckets</span><span class="sxs-lookup"><span data-stu-id="be0ee-136">buckets</span></span>|<span data-ttu-id="be0ee-137">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="be0ee-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="be0ee-p105">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="be0ee-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="be0ee-141">plans</span><span class="sxs-lookup"><span data-stu-id="be0ee-141">plans</span></span>|<span data-ttu-id="be0ee-142">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="be0ee-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="be0ee-p106">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="be0ee-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="be0ee-146">tasks</span><span class="sxs-lookup"><span data-stu-id="be0ee-146">tasks</span></span>|<span data-ttu-id="be0ee-147">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="be0ee-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="be0ee-p107">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="be0ee-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be0ee-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="be0ee-151">JSON representation</span></span>
<span data-ttu-id="be0ee-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be0ee-152">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->