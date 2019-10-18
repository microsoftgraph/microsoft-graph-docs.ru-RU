---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждому объекту plan соответствует объект details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1f928252963c7796a396e1e342b413d135fb1764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035184"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="b427b-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b427b-107">plannerPlan resource type</span></span>

<span data-ttu-id="b427b-108">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="b427b-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="b427b-109">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="b427b-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="b427b-110">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="b427b-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="b427b-111">Каждому объекту plan соответствует объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="b427b-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="b427b-112">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b427b-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b427b-113">Методы</span><span class="sxs-lookup"><span data-stu-id="b427b-113">Methods</span></span>

| <span data-ttu-id="b427b-114">Метод</span><span class="sxs-lookup"><span data-stu-id="b427b-114">Method</span></span>           | <span data-ttu-id="b427b-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b427b-115">Return Type</span></span>    |<span data-ttu-id="b427b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b427b-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b427b-117">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b427b-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="b427b-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b427b-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b427b-119">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="b427b-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="b427b-120">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="b427b-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="b427b-121">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="b427b-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b427b-122">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="b427b-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="b427b-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="b427b-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="b427b-124">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="b427b-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b427b-125">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="b427b-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="b427b-126">Обновление</span><span class="sxs-lookup"><span data-stu-id="b427b-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="b427b-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b427b-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b427b-128">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="b427b-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b427b-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b427b-129">Properties</span></span>
| <span data-ttu-id="b427b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b427b-130">Property</span></span>     | <span data-ttu-id="b427b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b427b-131">Type</span></span>   |<span data-ttu-id="b427b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b427b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b427b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b427b-133">createdDateTime</span></span>|<span data-ttu-id="b427b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b427b-134">DateTimeOffset</span></span>|<span data-ttu-id="b427b-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-135">Read-only.</span></span> <span data-ttu-id="b427b-136">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="b427b-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="b427b-137">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b427b-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b427b-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b427b-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b427b-139">id</span><span class="sxs-lookup"><span data-stu-id="b427b-139">id</span></span>|<span data-ttu-id="b427b-140">String</span><span class="sxs-lookup"><span data-stu-id="b427b-140">String</span></span>| <span data-ttu-id="b427b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-141">Read-only.</span></span> <span data-ttu-id="b427b-142">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="b427b-142">ID of the plan.</span></span> <span data-ttu-id="b427b-143">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="b427b-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b427b-144">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="b427b-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b427b-145">owner</span><span class="sxs-lookup"><span data-stu-id="b427b-145">owner</span></span>|<span data-ttu-id="b427b-146">String</span><span class="sxs-lookup"><span data-stu-id="b427b-146">String</span></span>|<span data-ttu-id="b427b-147">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="b427b-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="b427b-148">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="b427b-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="b427b-149">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="b427b-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="b427b-150">title</span><span class="sxs-lookup"><span data-stu-id="b427b-150">title</span></span>|<span data-ttu-id="b427b-151">String</span><span class="sxs-lookup"><span data-stu-id="b427b-151">String</span></span>|<span data-ttu-id="b427b-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b427b-152">Required.</span></span> <span data-ttu-id="b427b-153">Название плана.</span><span class="sxs-lookup"><span data-stu-id="b427b-153">Title of the plan.</span></span>|
|<span data-ttu-id="b427b-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="b427b-154">createdBy</span></span>|[<span data-ttu-id="b427b-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="b427b-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="b427b-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-156">Read-only.</span></span> <span data-ttu-id="b427b-157">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="b427b-157">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b427b-158">Связи</span><span class="sxs-lookup"><span data-stu-id="b427b-158">Relationships</span></span>
| <span data-ttu-id="b427b-159">Отношение</span><span class="sxs-lookup"><span data-stu-id="b427b-159">Relationship</span></span> | <span data-ttu-id="b427b-160">Тип</span><span class="sxs-lookup"><span data-stu-id="b427b-160">Type</span></span>   |<span data-ttu-id="b427b-161">Описание</span><span class="sxs-lookup"><span data-stu-id="b427b-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b427b-162">buckets</span><span class="sxs-lookup"><span data-stu-id="b427b-162">buckets</span></span>|<span data-ttu-id="b427b-163">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="b427b-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b427b-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-164">Read-only.</span></span> <span data-ttu-id="b427b-165">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="b427b-165">Nullable.</span></span> <span data-ttu-id="b427b-166">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="b427b-166">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="b427b-167">details</span><span class="sxs-lookup"><span data-stu-id="b427b-167">details</span></span>|[<span data-ttu-id="b427b-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b427b-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="b427b-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-169">Read-only.</span></span> <span data-ttu-id="b427b-170">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="b427b-170">Nullable.</span></span> <span data-ttu-id="b427b-171">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="b427b-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="b427b-172">tasks</span><span class="sxs-lookup"><span data-stu-id="b427b-172">tasks</span></span>|<span data-ttu-id="b427b-173">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="b427b-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b427b-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b427b-174">Read-only.</span></span> <span data-ttu-id="b427b-175">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="b427b-175">Nullable.</span></span> <span data-ttu-id="b427b-176">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="b427b-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b427b-177">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b427b-177">JSON representation</span></span>

<span data-ttu-id="b427b-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b427b-178">Here is a JSON representation of the resource.</span></span>

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
