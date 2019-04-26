---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждый объект Plan содержит объект Details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5da918e3ba0e8087d4572799168fa1132e0ce5e7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344468"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="41dd1-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="41dd1-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41dd1-108">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="41dd1-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="41dd1-109">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="41dd1-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="41dd1-110">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="41dd1-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="41dd1-111">Каждый объект Plan содержит объект [Details](plannerplandetails.md) , который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="41dd1-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="41dd1-112">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="41dd1-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="41dd1-113">Методы</span><span class="sxs-lookup"><span data-stu-id="41dd1-113">Methods</span></span>

| <span data-ttu-id="41dd1-114">Метод</span><span class="sxs-lookup"><span data-stu-id="41dd1-114">Method</span></span>           | <span data-ttu-id="41dd1-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="41dd1-115">Return Type</span></span>    |<span data-ttu-id="41dd1-116">Описание</span><span class="sxs-lookup"><span data-stu-id="41dd1-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41dd1-117">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="41dd1-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="41dd1-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="41dd1-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="41dd1-119">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="41dd1-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="41dd1-120">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="41dd1-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="41dd1-121">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="41dd1-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="41dd1-122">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="41dd1-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="41dd1-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="41dd1-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="41dd1-124">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="41dd1-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="41dd1-125">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="41dd1-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="41dd1-126">Обновление</span><span class="sxs-lookup"><span data-stu-id="41dd1-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="41dd1-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="41dd1-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="41dd1-128">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="41dd1-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41dd1-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="41dd1-129">Properties</span></span>
| <span data-ttu-id="41dd1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41dd1-130">Property</span></span>     | <span data-ttu-id="41dd1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41dd1-131">Type</span></span>   |<span data-ttu-id="41dd1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41dd1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41dd1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41dd1-133">createdDateTime</span></span>|<span data-ttu-id="41dd1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41dd1-134">DateTimeOffset</span></span>|<span data-ttu-id="41dd1-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-135">Read-only.</span></span> <span data-ttu-id="41dd1-136">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="41dd1-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="41dd1-137">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="41dd1-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41dd1-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="41dd1-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="41dd1-139">id</span><span class="sxs-lookup"><span data-stu-id="41dd1-139">id</span></span>|<span data-ttu-id="41dd1-140">String</span><span class="sxs-lookup"><span data-stu-id="41dd1-140">String</span></span>| <span data-ttu-id="41dd1-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-141">Read-only.</span></span> <span data-ttu-id="41dd1-142">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="41dd1-142">ID of the plan.</span></span> <span data-ttu-id="41dd1-143">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="41dd1-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="41dd1-144">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="41dd1-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="41dd1-145">owner</span><span class="sxs-lookup"><span data-stu-id="41dd1-145">owner</span></span>|<span data-ttu-id="41dd1-146">String</span><span class="sxs-lookup"><span data-stu-id="41dd1-146">String</span></span>|<span data-ttu-id="41dd1-147">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="41dd1-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="41dd1-148">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="41dd1-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="41dd1-149">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="41dd1-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="41dd1-150">title</span><span class="sxs-lookup"><span data-stu-id="41dd1-150">title</span></span>|<span data-ttu-id="41dd1-151">String</span><span class="sxs-lookup"><span data-stu-id="41dd1-151">String</span></span>|<span data-ttu-id="41dd1-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41dd1-152">Required.</span></span> <span data-ttu-id="41dd1-153">Название плана.</span><span class="sxs-lookup"><span data-stu-id="41dd1-153">Title of the plan.</span></span>|
|<span data-ttu-id="41dd1-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="41dd1-154">createdBy</span></span>|[<span data-ttu-id="41dd1-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="41dd1-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="41dd1-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-156">Read-only.</span></span> <span data-ttu-id="41dd1-157">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="41dd1-157">The user who created the plan.</span></span>|
|<span data-ttu-id="41dd1-158">контекстах</span><span class="sxs-lookup"><span data-stu-id="41dd1-158">contexts</span></span>|<span data-ttu-id="41dd1-159">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="41dd1-159">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="41dd1-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-160">Read-only.</span></span> <span data-ttu-id="41dd1-161">Дополнительные пользовательские взаимодействия, в которых используется этот план, представленный в виде записей [планнерпланконтекст](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="41dd1-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41dd1-162">Связи</span><span class="sxs-lookup"><span data-stu-id="41dd1-162">Relationships</span></span>
| <span data-ttu-id="41dd1-163">Отношение</span><span class="sxs-lookup"><span data-stu-id="41dd1-163">Relationship</span></span> | <span data-ttu-id="41dd1-164">Тип</span><span class="sxs-lookup"><span data-stu-id="41dd1-164">Type</span></span>   |<span data-ttu-id="41dd1-165">Описание</span><span class="sxs-lookup"><span data-stu-id="41dd1-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41dd1-166">buckets</span><span class="sxs-lookup"><span data-stu-id="41dd1-166">buckets</span></span>|<span data-ttu-id="41dd1-167">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="41dd1-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="41dd1-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-168">Read-only.</span></span> <span data-ttu-id="41dd1-169">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="41dd1-169">Nullable.</span></span> <span data-ttu-id="41dd1-170">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="41dd1-170">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="41dd1-171">details</span><span class="sxs-lookup"><span data-stu-id="41dd1-171">details</span></span>|[<span data-ttu-id="41dd1-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="41dd1-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="41dd1-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-173">Read-only.</span></span> <span data-ttu-id="41dd1-174">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="41dd1-174">Nullable.</span></span> <span data-ttu-id="41dd1-175">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="41dd1-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="41dd1-176">tasks</span><span class="sxs-lookup"><span data-stu-id="41dd1-176">tasks</span></span>|<span data-ttu-id="41dd1-177">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="41dd1-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="41dd1-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41dd1-178">Read-only.</span></span> <span data-ttu-id="41dd1-179">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="41dd1-179">Nullable.</span></span> <span data-ttu-id="41dd1-180">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="41dd1-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41dd1-181">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="41dd1-181">JSON representation</span></span>

<span data-ttu-id="41dd1-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41dd1-182">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
