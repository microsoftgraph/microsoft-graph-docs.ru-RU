---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждый объект Plan содержит объект Details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 386eff2e771967231a5c37d73ea913252e5d3324
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979343"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="d816b-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d816b-107">plannerPlan resource type</span></span>

<span data-ttu-id="d816b-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d816b-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d816b-109">Ресурс **plannerPlan** представляет план в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d816b-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="d816b-110">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="d816b-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="d816b-111">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="d816b-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="d816b-112">Каждый объект Plan содержит объект [Details](plannerplandetails.md) , который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="d816b-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="d816b-113">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d816b-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="d816b-114">Методы</span><span class="sxs-lookup"><span data-stu-id="d816b-114">Methods</span></span>

| <span data-ttu-id="d816b-115">Метод</span><span class="sxs-lookup"><span data-stu-id="d816b-115">Method</span></span>           | <span data-ttu-id="d816b-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d816b-116">Return Type</span></span>    |<span data-ttu-id="d816b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d816b-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d816b-118">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d816b-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="d816b-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d816b-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="d816b-120">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d816b-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="d816b-121">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="d816b-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="d816b-122">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d816b-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d816b-123">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="d816b-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="d816b-124">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="d816b-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="d816b-125">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d816b-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d816b-126">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="d816b-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="d816b-127">Обновление</span><span class="sxs-lookup"><span data-stu-id="d816b-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="d816b-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d816b-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="d816b-129">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d816b-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d816b-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="d816b-130">Properties</span></span>
| <span data-ttu-id="d816b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d816b-131">Property</span></span>     | <span data-ttu-id="d816b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d816b-132">Type</span></span>   |<span data-ttu-id="d816b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d816b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d816b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d816b-134">createdDateTime</span></span>|<span data-ttu-id="d816b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d816b-135">DateTimeOffset</span></span>|<span data-ttu-id="d816b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-136">Read-only.</span></span> <span data-ttu-id="d816b-137">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="d816b-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="d816b-138">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d816b-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d816b-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d816b-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d816b-140">id</span><span class="sxs-lookup"><span data-stu-id="d816b-140">id</span></span>|<span data-ttu-id="d816b-141">String</span><span class="sxs-lookup"><span data-stu-id="d816b-141">String</span></span>| <span data-ttu-id="d816b-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-142">Read-only.</span></span> <span data-ttu-id="d816b-143">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="d816b-143">ID of the plan.</span></span> <span data-ttu-id="d816b-144">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="d816b-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d816b-145">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="d816b-145">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d816b-146">owner</span><span class="sxs-lookup"><span data-stu-id="d816b-146">owner</span></span>|<span data-ttu-id="d816b-147">String</span><span class="sxs-lookup"><span data-stu-id="d816b-147">String</span></span>|<span data-ttu-id="d816b-148">Идентификатор [группы](group.md), которая является владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="d816b-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="d816b-149">Чтобы в этом поле можно было указать значение, должна существовать подходящая группа.</span><span class="sxs-lookup"><span data-stu-id="d816b-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="d816b-150">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="d816b-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="d816b-151">title</span><span class="sxs-lookup"><span data-stu-id="d816b-151">title</span></span>|<span data-ttu-id="d816b-152">String</span><span class="sxs-lookup"><span data-stu-id="d816b-152">String</span></span>|<span data-ttu-id="d816b-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d816b-153">Required.</span></span> <span data-ttu-id="d816b-154">Название плана.</span><span class="sxs-lookup"><span data-stu-id="d816b-154">Title of the plan.</span></span>|
|<span data-ttu-id="d816b-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="d816b-155">createdBy</span></span>|[<span data-ttu-id="d816b-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="d816b-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="d816b-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-157">Read-only.</span></span> <span data-ttu-id="d816b-158">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="d816b-158">The user who created the plan.</span></span>|
|<span data-ttu-id="d816b-159">контекстах</span><span class="sxs-lookup"><span data-stu-id="d816b-159">contexts</span></span>|<span data-ttu-id="d816b-160">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="d816b-160">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="d816b-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-161">Read-only.</span></span> <span data-ttu-id="d816b-162">Дополнительные пользовательские взаимодействия, в которых используется этот план, представленный в виде записей [планнерпланконтекст](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="d816b-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d816b-163">Связи</span><span class="sxs-lookup"><span data-stu-id="d816b-163">Relationships</span></span>
| <span data-ttu-id="d816b-164">Связь</span><span class="sxs-lookup"><span data-stu-id="d816b-164">Relationship</span></span> | <span data-ttu-id="d816b-165">Тип</span><span class="sxs-lookup"><span data-stu-id="d816b-165">Type</span></span>   |<span data-ttu-id="d816b-166">Описание</span><span class="sxs-lookup"><span data-stu-id="d816b-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d816b-167">buckets</span><span class="sxs-lookup"><span data-stu-id="d816b-167">buckets</span></span>|<span data-ttu-id="d816b-168">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d816b-168">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d816b-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-169">Read-only.</span></span> <span data-ttu-id="d816b-170">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="d816b-170">Nullable.</span></span> <span data-ttu-id="d816b-171">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="d816b-171">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="d816b-172">details</span><span class="sxs-lookup"><span data-stu-id="d816b-172">details</span></span>|[<span data-ttu-id="d816b-173">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d816b-173">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="d816b-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-174">Read-only.</span></span> <span data-ttu-id="d816b-175">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="d816b-175">Nullable.</span></span> <span data-ttu-id="d816b-176">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="d816b-176">Additional details about the plan.</span></span>|
|<span data-ttu-id="d816b-177">tasks</span><span class="sxs-lookup"><span data-stu-id="d816b-177">tasks</span></span>|<span data-ttu-id="d816b-178">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d816b-178">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d816b-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d816b-179">Read-only.</span></span> <span data-ttu-id="d816b-180">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="d816b-180">Nullable.</span></span> <span data-ttu-id="d816b-181">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="d816b-181">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d816b-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d816b-182">JSON representation</span></span>

<span data-ttu-id="d816b-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d816b-183">Here is a JSON representation of the resource.</span></span>

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


