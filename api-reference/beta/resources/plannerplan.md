---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждый объект Plan содержит объект Details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e1dfc5e7c51bdb902b4c2c5f16c90eeb6b1e7771
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898256"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="065da-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="065da-107">plannerPlan resource type</span></span>

<span data-ttu-id="065da-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="065da-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="065da-109">Ресурс **plannerPlan** представляет план в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="065da-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="065da-110">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="065da-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="065da-111">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="065da-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="065da-112">Каждый объект Plan содержит объект [Details](plannerplandetails.md) , который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="065da-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="065da-113">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="065da-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="065da-114">Методы</span><span class="sxs-lookup"><span data-stu-id="065da-114">Methods</span></span>

| <span data-ttu-id="065da-115">Метод</span><span class="sxs-lookup"><span data-stu-id="065da-115">Method</span></span>           | <span data-ttu-id="065da-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="065da-116">Return Type</span></span>    |<span data-ttu-id="065da-117">Описание</span><span class="sxs-lookup"><span data-stu-id="065da-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="065da-118">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="065da-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="065da-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="065da-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="065da-120">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="065da-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="065da-121">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="065da-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="065da-122">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="065da-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="065da-123">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="065da-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="065da-124">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="065da-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="065da-125">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="065da-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="065da-126">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="065da-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="065da-127">Обновление</span><span class="sxs-lookup"><span data-stu-id="065da-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="065da-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="065da-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="065da-129">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="065da-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="065da-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="065da-130">Properties</span></span>
| <span data-ttu-id="065da-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="065da-131">Property</span></span>     | <span data-ttu-id="065da-132">Тип</span><span class="sxs-lookup"><span data-stu-id="065da-132">Type</span></span>   |<span data-ttu-id="065da-133">Описание</span><span class="sxs-lookup"><span data-stu-id="065da-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="065da-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="065da-134">createdDateTime</span></span>|<span data-ttu-id="065da-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="065da-135">DateTimeOffset</span></span>|<span data-ttu-id="065da-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-136">Read-only.</span></span> <span data-ttu-id="065da-137">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="065da-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="065da-138">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="065da-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="065da-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="065da-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="065da-140">id</span><span class="sxs-lookup"><span data-stu-id="065da-140">id</span></span>|<span data-ttu-id="065da-141">String</span><span class="sxs-lookup"><span data-stu-id="065da-141">String</span></span>| <span data-ttu-id="065da-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-142">Read-only.</span></span> <span data-ttu-id="065da-143">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="065da-143">ID of the plan.</span></span> <span data-ttu-id="065da-144">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="065da-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="065da-145">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="065da-145">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="065da-146">owner</span><span class="sxs-lookup"><span data-stu-id="065da-146">owner</span></span>|<span data-ttu-id="065da-147">String</span><span class="sxs-lookup"><span data-stu-id="065da-147">String</span></span>|<span data-ttu-id="065da-148">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="065da-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="065da-149">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="065da-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="065da-150">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="065da-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="065da-151">title</span><span class="sxs-lookup"><span data-stu-id="065da-151">title</span></span>|<span data-ttu-id="065da-152">String</span><span class="sxs-lookup"><span data-stu-id="065da-152">String</span></span>|<span data-ttu-id="065da-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="065da-153">Required.</span></span> <span data-ttu-id="065da-154">Название плана.</span><span class="sxs-lookup"><span data-stu-id="065da-154">Title of the plan.</span></span>|
|<span data-ttu-id="065da-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="065da-155">createdBy</span></span>|[<span data-ttu-id="065da-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="065da-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="065da-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-157">Read-only.</span></span> <span data-ttu-id="065da-158">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="065da-158">The user who created the plan.</span></span>|
|<span data-ttu-id="065da-159">контекстах</span><span class="sxs-lookup"><span data-stu-id="065da-159">contexts</span></span>|<span data-ttu-id="065da-160">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="065da-160">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="065da-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-161">Read-only.</span></span> <span data-ttu-id="065da-162">Дополнительные пользовательские взаимодействия, в которых используется этот план, представленный в виде записей [планнерпланконтекст](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="065da-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="065da-163">Связи</span><span class="sxs-lookup"><span data-stu-id="065da-163">Relationships</span></span>
| <span data-ttu-id="065da-164">Связь</span><span class="sxs-lookup"><span data-stu-id="065da-164">Relationship</span></span> | <span data-ttu-id="065da-165">Тип</span><span class="sxs-lookup"><span data-stu-id="065da-165">Type</span></span>   |<span data-ttu-id="065da-166">Описание</span><span class="sxs-lookup"><span data-stu-id="065da-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="065da-167">buckets</span><span class="sxs-lookup"><span data-stu-id="065da-167">buckets</span></span>|<span data-ttu-id="065da-168">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="065da-168">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="065da-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-169">Read-only.</span></span> <span data-ttu-id="065da-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="065da-170">Nullable.</span></span> <span data-ttu-id="065da-171">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="065da-171">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="065da-172">details</span><span class="sxs-lookup"><span data-stu-id="065da-172">details</span></span>|[<span data-ttu-id="065da-173">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="065da-173">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="065da-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-174">Read-only.</span></span> <span data-ttu-id="065da-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="065da-175">Nullable.</span></span> <span data-ttu-id="065da-176">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="065da-176">Additional details about the plan.</span></span>|
|<span data-ttu-id="065da-177">tasks</span><span class="sxs-lookup"><span data-stu-id="065da-177">tasks</span></span>|<span data-ttu-id="065da-178">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="065da-178">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="065da-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065da-179">Read-only.</span></span> <span data-ttu-id="065da-180">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="065da-180">Nullable.</span></span> <span data-ttu-id="065da-181">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="065da-181">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="065da-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="065da-182">JSON representation</span></span>

<span data-ttu-id="065da-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="065da-183">Here is a JSON representation of the resource.</span></span>

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
