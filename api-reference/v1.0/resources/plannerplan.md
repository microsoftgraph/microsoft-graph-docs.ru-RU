---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержит коллекцию plannerTasks. Он также может иметь коллекцию plannerBuckets. Каждый объект плана имеет объект сведений, который может содержать дополнительные сведения о плане. Дополнительные сведения о связях между группами, планы и задачи можно планировщик работы.
localization_priority: Priority
ms.openlocfilehash: cfcc94fab067cc76bb530edbdb8477183ebf3531
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873012"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="bc6d5-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bc6d5-107">plannerPlan resource type</span></span>

<span data-ttu-id="bc6d5-p102">Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md). Каждый объект plan имеет объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p102">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md). It can also have a collection of [plannerBuckets](plannerbucket.md). Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bc6d5-113">Методы</span><span class="sxs-lookup"><span data-stu-id="bc6d5-113">Methods</span></span>

| <span data-ttu-id="bc6d5-114">Метод</span><span class="sxs-lookup"><span data-stu-id="bc6d5-114">Method</span></span>           | <span data-ttu-id="bc6d5-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc6d5-115">Return Type</span></span>    |<span data-ttu-id="bc6d5-116">Описание</span><span class="sxs-lookup"><span data-stu-id="bc6d5-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc6d5-117">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bc6d5-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="bc6d5-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bc6d5-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="bc6d5-119">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="bc6d5-120">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="bc6d5-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="bc6d5-121">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="bc6d5-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="bc6d5-122">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="bc6d5-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="bc6d5-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="bc6d5-124">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="bc6d5-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bc6d5-125">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-125">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="bc6d5-126">[обновление](../api/plannerplan-update.md).</span><span class="sxs-lookup"><span data-stu-id="bc6d5-126">[Update](../api/plannerplan-update.md)</span></span> | [<span data-ttu-id="bc6d5-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="bc6d5-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="bc6d5-128">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc6d5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc6d5-129">Properties</span></span>
| <span data-ttu-id="bc6d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc6d5-130">Property</span></span>     | <span data-ttu-id="bc6d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc6d5-131">Type</span></span>   |<span data-ttu-id="bc6d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc6d5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc6d5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc6d5-133">createdDateTime</span></span>|<span data-ttu-id="bc6d5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc6d5-134">DateTimeOffset</span></span>|<span data-ttu-id="bc6d5-p103">Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bc6d5-139">id</span><span class="sxs-lookup"><span data-stu-id="bc6d5-139">id</span></span>|<span data-ttu-id="bc6d5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bc6d5-140">String</span></span>| <span data-ttu-id="bc6d5-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-141">Read-only.</span></span> <span data-ttu-id="bc6d5-142">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-142">ID of the plan.</span></span> <span data-ttu-id="bc6d5-143">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="bc6d5-144">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="bc6d5-145">owner</span><span class="sxs-lookup"><span data-stu-id="bc6d5-145">owner</span></span>|<span data-ttu-id="bc6d5-146">Строка</span><span class="sxs-lookup"><span data-stu-id="bc6d5-146">String</span></span>|<span data-ttu-id="bc6d5-147">Идентификатор [группы](group.md) , который несет ответственность за планирование.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="bc6d5-148">В этом поле можно указать допустимое группы должен существовать.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="bc6d5-149">После его установки, это свойство не удается обновить.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="bc6d5-150">title</span><span class="sxs-lookup"><span data-stu-id="bc6d5-150">title</span></span>|<span data-ttu-id="bc6d5-151">String</span><span class="sxs-lookup"><span data-stu-id="bc6d5-151">String</span></span>|<span data-ttu-id="bc6d5-p106">Обязательный. Название плана.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="bc6d5-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="bc6d5-154">createdBy</span></span>|[<span data-ttu-id="bc6d5-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="bc6d5-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="bc6d5-p107">Только для чтения. Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p107">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc6d5-158">Связи</span><span class="sxs-lookup"><span data-stu-id="bc6d5-158">Relationships</span></span>
| <span data-ttu-id="bc6d5-159">Связь</span><span class="sxs-lookup"><span data-stu-id="bc6d5-159">Relationship</span></span> | <span data-ttu-id="bc6d5-160">Тип</span><span class="sxs-lookup"><span data-stu-id="bc6d5-160">Type</span></span>   |<span data-ttu-id="bc6d5-161">Описание</span><span class="sxs-lookup"><span data-stu-id="bc6d5-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc6d5-162">buckets</span><span class="sxs-lookup"><span data-stu-id="bc6d5-162">buckets</span></span>|<span data-ttu-id="bc6d5-163">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="bc6d5-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="bc6d5-p108">Только для чтения. Допускает значение null. Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="bc6d5-167">details</span><span class="sxs-lookup"><span data-stu-id="bc6d5-167">details</span></span>|<span data-ttu-id="bc6d5-168">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="bc6d5-168">[plannerPlanDetails](plannerplandetails.md)</span></span>| <span data-ttu-id="bc6d5-p109">Только для чтения. Допускает значение null. Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p109">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="bc6d5-172">tasks</span><span class="sxs-lookup"><span data-stu-id="bc6d5-172">tasks</span></span>|<span data-ttu-id="bc6d5-173">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="bc6d5-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bc6d5-p110">Только для чтения. Допускает значение null. Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-p110">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc6d5-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc6d5-177">JSON representation</span></span>

<span data-ttu-id="bc6d5-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc6d5-178">Here is a JSON representation of the resource.</span></span>

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
