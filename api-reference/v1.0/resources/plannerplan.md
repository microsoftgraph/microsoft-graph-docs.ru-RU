---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждому объекту plan соответствует объект details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea9ef53ee472c9051be6baabe35dc2a0a03e620f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533990"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="667da-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="667da-107">plannerPlan resource type</span></span>

<span data-ttu-id="667da-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="667da-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="667da-109">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="667da-109">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="667da-110">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="667da-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="667da-111">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="667da-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="667da-112">Каждому объекту plan соответствует объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="667da-112">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="667da-113">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="667da-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="667da-114">Методы</span><span class="sxs-lookup"><span data-stu-id="667da-114">Methods</span></span>

| <span data-ttu-id="667da-115">Метод</span><span class="sxs-lookup"><span data-stu-id="667da-115">Method</span></span>           | <span data-ttu-id="667da-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="667da-116">Return Type</span></span>    |<span data-ttu-id="667da-117">Описание</span><span class="sxs-lookup"><span data-stu-id="667da-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="667da-118">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="667da-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="667da-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="667da-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="667da-120">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="667da-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="667da-121">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="667da-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="667da-122">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="667da-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="667da-123">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="667da-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="667da-124">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="667da-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="667da-125">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="667da-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="667da-126">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="667da-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="667da-127">Обновление</span><span class="sxs-lookup"><span data-stu-id="667da-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="667da-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="667da-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="667da-129">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="667da-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="667da-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="667da-130">Properties</span></span>
| <span data-ttu-id="667da-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="667da-131">Property</span></span>     | <span data-ttu-id="667da-132">Тип</span><span class="sxs-lookup"><span data-stu-id="667da-132">Type</span></span>   |<span data-ttu-id="667da-133">Описание</span><span class="sxs-lookup"><span data-stu-id="667da-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667da-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="667da-134">createdDateTime</span></span>|<span data-ttu-id="667da-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667da-135">DateTimeOffset</span></span>|<span data-ttu-id="667da-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-136">Read-only.</span></span> <span data-ttu-id="667da-137">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="667da-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="667da-138">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="667da-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="667da-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="667da-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="667da-140">id</span><span class="sxs-lookup"><span data-stu-id="667da-140">id</span></span>|<span data-ttu-id="667da-141">String</span><span class="sxs-lookup"><span data-stu-id="667da-141">String</span></span>| <span data-ttu-id="667da-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-142">Read-only.</span></span> <span data-ttu-id="667da-143">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="667da-143">ID of the plan.</span></span> <span data-ttu-id="667da-144">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="667da-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="667da-145">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="667da-145">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="667da-146">owner</span><span class="sxs-lookup"><span data-stu-id="667da-146">owner</span></span>|<span data-ttu-id="667da-147">String</span><span class="sxs-lookup"><span data-stu-id="667da-147">String</span></span>|<span data-ttu-id="667da-148">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="667da-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="667da-149">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="667da-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="667da-150">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="667da-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="667da-151">title</span><span class="sxs-lookup"><span data-stu-id="667da-151">title</span></span>|<span data-ttu-id="667da-152">String</span><span class="sxs-lookup"><span data-stu-id="667da-152">String</span></span>|<span data-ttu-id="667da-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667da-153">Required.</span></span> <span data-ttu-id="667da-154">Название плана.</span><span class="sxs-lookup"><span data-stu-id="667da-154">Title of the plan.</span></span>|
|<span data-ttu-id="667da-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="667da-155">createdBy</span></span>|[<span data-ttu-id="667da-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="667da-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="667da-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-157">Read-only.</span></span> <span data-ttu-id="667da-158">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="667da-158">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="667da-159">Связи</span><span class="sxs-lookup"><span data-stu-id="667da-159">Relationships</span></span>
| <span data-ttu-id="667da-160">Связь</span><span class="sxs-lookup"><span data-stu-id="667da-160">Relationship</span></span> | <span data-ttu-id="667da-161">Тип</span><span class="sxs-lookup"><span data-stu-id="667da-161">Type</span></span>   |<span data-ttu-id="667da-162">Описание</span><span class="sxs-lookup"><span data-stu-id="667da-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667da-163">buckets</span><span class="sxs-lookup"><span data-stu-id="667da-163">buckets</span></span>|<span data-ttu-id="667da-164">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="667da-164">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="667da-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-165">Read-only.</span></span> <span data-ttu-id="667da-166">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="667da-166">Nullable.</span></span> <span data-ttu-id="667da-167">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="667da-167">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="667da-168">details</span><span class="sxs-lookup"><span data-stu-id="667da-168">details</span></span>|[<span data-ttu-id="667da-169">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="667da-169">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="667da-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-170">Read-only.</span></span> <span data-ttu-id="667da-171">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="667da-171">Nullable.</span></span> <span data-ttu-id="667da-172">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="667da-172">Additional details about the plan.</span></span>|
|<span data-ttu-id="667da-173">tasks</span><span class="sxs-lookup"><span data-stu-id="667da-173">tasks</span></span>|<span data-ttu-id="667da-174">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="667da-174">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="667da-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667da-175">Read-only.</span></span> <span data-ttu-id="667da-176">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="667da-176">Nullable.</span></span> <span data-ttu-id="667da-177">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="667da-177">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="667da-178">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="667da-178">JSON representation</span></span>

<span data-ttu-id="667da-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667da-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
