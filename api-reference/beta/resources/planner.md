---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
localization_priority: Normal
ms.openlocfilehash: 9dc6904da25d7612b94649264001dcae98859925
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889098"
---
# <a name="planner-resource-type"></a><span data-ttu-id="b8899-105">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="b8899-105">planner resource type</span></span>

> <span data-ttu-id="b8899-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8899-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8899-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8899-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8899-p103">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="b8899-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="b8899-111">Методы</span><span class="sxs-lookup"><span data-stu-id="b8899-111">Methods</span></span>

| <span data-ttu-id="b8899-112">Метод</span><span class="sxs-lookup"><span data-stu-id="b8899-112">Method</span></span>           | <span data-ttu-id="b8899-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8899-113">Return Type</span></span>    |<span data-ttu-id="b8899-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b8899-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8899-115">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b8899-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="b8899-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b8899-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="b8899-117">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="b8899-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="b8899-118">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b8899-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="b8899-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b8899-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="b8899-120">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="b8899-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="b8899-121">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="b8899-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="b8899-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="b8899-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="b8899-123">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="b8899-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8899-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8899-124">Properties</span></span>
| <span data-ttu-id="b8899-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8899-125">Property</span></span>     | <span data-ttu-id="b8899-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b8899-126">Type</span></span>   |<span data-ttu-id="b8899-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b8899-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8899-128">id</span><span class="sxs-lookup"><span data-stu-id="b8899-128">id</span></span>|<span data-ttu-id="b8899-129">String</span><span class="sxs-lookup"><span data-stu-id="b8899-129">String</span></span>| <span data-ttu-id="b8899-p104">Только для чтения. Идентификатор ресурса **planner**.</span><span class="sxs-lookup"><span data-stu-id="b8899-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8899-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b8899-132">Relationships</span></span>
| <span data-ttu-id="b8899-133">Связь</span><span class="sxs-lookup"><span data-stu-id="b8899-133">Relationship</span></span> | <span data-ttu-id="b8899-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b8899-134">Type</span></span>   |<span data-ttu-id="b8899-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b8899-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8899-136">buckets</span><span class="sxs-lookup"><span data-stu-id="b8899-136">buckets</span></span>|<span data-ttu-id="b8899-137">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="b8899-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b8899-p105">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="b8899-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="b8899-141">plans</span><span class="sxs-lookup"><span data-stu-id="b8899-141">plans</span></span>|<span data-ttu-id="b8899-142">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="b8899-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b8899-p106">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="b8899-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="b8899-146">tasks</span><span class="sxs-lookup"><span data-stu-id="b8899-146">tasks</span></span>|<span data-ttu-id="b8899-147">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="b8899-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b8899-p107">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="b8899-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8899-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b8899-151">JSON representation</span></span>
<span data-ttu-id="b8899-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8899-152">Here is a JSON representation of the resource.</span></span>

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
