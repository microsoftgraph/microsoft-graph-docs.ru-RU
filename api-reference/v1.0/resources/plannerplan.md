---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждому объекту plan соответствует объект details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9e77f2c0163f9093d931c46098498caa8c43f42c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462293"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="e53b7-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e53b7-107">plannerPlan resource type</span></span>

<span data-ttu-id="e53b7-108">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="e53b7-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="e53b7-109">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="e53b7-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="e53b7-110">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="e53b7-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="e53b7-111">Каждому объекту plan соответствует объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="e53b7-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="e53b7-112">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e53b7-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e53b7-113">Методы</span><span class="sxs-lookup"><span data-stu-id="e53b7-113">Methods</span></span>

| <span data-ttu-id="e53b7-114">Метод</span><span class="sxs-lookup"><span data-stu-id="e53b7-114">Method</span></span>           | <span data-ttu-id="e53b7-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e53b7-115">Return Type</span></span>    |<span data-ttu-id="e53b7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e53b7-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e53b7-117">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e53b7-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="e53b7-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e53b7-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e53b7-119">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="e53b7-119">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="e53b7-120">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="e53b7-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="e53b7-121">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="e53b7-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e53b7-122">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="e53b7-122">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="e53b7-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="e53b7-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="e53b7-124">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="e53b7-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e53b7-125">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="e53b7-125">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="e53b7-126">Обновление</span><span class="sxs-lookup"><span data-stu-id="e53b7-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="e53b7-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e53b7-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e53b7-128">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="e53b7-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e53b7-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e53b7-129">Properties</span></span>
| <span data-ttu-id="e53b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e53b7-130">Property</span></span>     | <span data-ttu-id="e53b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e53b7-131">Type</span></span>   |<span data-ttu-id="e53b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e53b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53b7-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e53b7-133">createdDateTime</span></span>|<span data-ttu-id="e53b7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53b7-134">DateTimeOffset</span></span>|<span data-ttu-id="e53b7-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-135">Read-only.</span></span> <span data-ttu-id="e53b7-136">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="e53b7-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="e53b7-137">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e53b7-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e53b7-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e53b7-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e53b7-139">id</span><span class="sxs-lookup"><span data-stu-id="e53b7-139">id</span></span>|<span data-ttu-id="e53b7-140">String</span><span class="sxs-lookup"><span data-stu-id="e53b7-140">String</span></span>| <span data-ttu-id="e53b7-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-141">Read-only.</span></span> <span data-ttu-id="e53b7-142">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="e53b7-142">ID of the message</span></span> <span data-ttu-id="e53b7-143">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e53b7-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e53b7-144">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="e53b7-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e53b7-145">owner</span><span class="sxs-lookup"><span data-stu-id="e53b7-145">owner</span></span>|<span data-ttu-id="e53b7-146">String</span><span class="sxs-lookup"><span data-stu-id="e53b7-146">String</span></span>|<span data-ttu-id="e53b7-147">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="e53b7-147">ID of the principal that owns the lock.</span></span> <span data-ttu-id="e53b7-148">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="e53b7-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="e53b7-149">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="e53b7-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="e53b7-150">title</span><span class="sxs-lookup"><span data-stu-id="e53b7-150">title</span></span>|<span data-ttu-id="e53b7-151">String</span><span class="sxs-lookup"><span data-stu-id="e53b7-151">String</span></span>|<span data-ttu-id="e53b7-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e53b7-152">Required.</span></span> <span data-ttu-id="e53b7-153">Название плана.</span><span class="sxs-lookup"><span data-stu-id="e53b7-153">Title of the plan.</span></span>|
|<span data-ttu-id="e53b7-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="e53b7-154">createdBy</span></span>|[<span data-ttu-id="e53b7-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="e53b7-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="e53b7-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-156">Read-only.</span></span> <span data-ttu-id="e53b7-157">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="e53b7-157">The user who created the Timesheet is listed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e53b7-158">Связи</span><span class="sxs-lookup"><span data-stu-id="e53b7-158">Relationships</span></span>
| <span data-ttu-id="e53b7-159">Отношение</span><span class="sxs-lookup"><span data-stu-id="e53b7-159">Relationship</span></span> | <span data-ttu-id="e53b7-160">Тип</span><span class="sxs-lookup"><span data-stu-id="e53b7-160">Type</span></span>   |<span data-ttu-id="e53b7-161">Описание</span><span class="sxs-lookup"><span data-stu-id="e53b7-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53b7-162">buckets</span><span class="sxs-lookup"><span data-stu-id="e53b7-162">Buckets</span></span>|<span data-ttu-id="e53b7-163">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="e53b7-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e53b7-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-164">Read-only.</span></span> <span data-ttu-id="e53b7-165">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="e53b7-165">Nullable.</span></span> <span data-ttu-id="e53b7-166">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="e53b7-166">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="e53b7-167">details</span><span class="sxs-lookup"><span data-stu-id="e53b7-167">details</span></span>|[<span data-ttu-id="e53b7-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e53b7-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="e53b7-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-169">Read-only.</span></span> <span data-ttu-id="e53b7-170">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="e53b7-170">Nullable.</span></span> <span data-ttu-id="e53b7-171">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="e53b7-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="e53b7-172">tasks</span><span class="sxs-lookup"><span data-stu-id="e53b7-172">tasks</span></span>|<span data-ttu-id="e53b7-173">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="e53b7-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e53b7-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e53b7-174">Read-only.</span></span> <span data-ttu-id="e53b7-175">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="e53b7-175">Nullable.</span></span> <span data-ttu-id="e53b7-176">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="e53b7-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e53b7-177">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e53b7-177">JSON representation</span></span>

<span data-ttu-id="e53b7-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e53b7-178">Here is a JSON representation of the resource.</span></span>

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
