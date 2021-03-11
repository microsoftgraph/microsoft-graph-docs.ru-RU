---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждый объект плана имеет объект подробностей, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4763f268628a4609ac91d0597aeb4f55a2d406ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720993"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="efeaa-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="efeaa-107">plannerPlan resource type</span></span>

<span data-ttu-id="efeaa-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efeaa-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efeaa-109">Ресурс **plannerPlan** представляет план в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="efeaa-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="efeaa-110">План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="efeaa-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="efeaa-111">Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="efeaa-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="efeaa-112">Каждый объект плана имеет объект [подробностей,](plannerplandetails.md) который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="efeaa-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="efeaa-113">Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="efeaa-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="efeaa-114">Методы</span><span class="sxs-lookup"><span data-stu-id="efeaa-114">Methods</span></span>

| <span data-ttu-id="efeaa-115">Метод</span><span class="sxs-lookup"><span data-stu-id="efeaa-115">Method</span></span>           | <span data-ttu-id="efeaa-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efeaa-116">Return Type</span></span>    |<span data-ttu-id="efeaa-117">Описание</span><span class="sxs-lookup"><span data-stu-id="efeaa-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efeaa-118">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="efeaa-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="efeaa-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="efeaa-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="efeaa-120">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="efeaa-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="efeaa-121">Перечисление контейнеров</span><span class="sxs-lookup"><span data-stu-id="efeaa-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="efeaa-122">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="efeaa-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="efeaa-123">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="efeaa-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="efeaa-124">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="efeaa-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="efeaa-125">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="efeaa-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="efeaa-126">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="efeaa-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="efeaa-127">Обновление</span><span class="sxs-lookup"><span data-stu-id="efeaa-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="efeaa-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="efeaa-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="efeaa-129">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="efeaa-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="efeaa-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="efeaa-130">Properties</span></span>
| <span data-ttu-id="efeaa-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="efeaa-131">Property</span></span>     | <span data-ttu-id="efeaa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="efeaa-132">Type</span></span>   |<span data-ttu-id="efeaa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="efeaa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efeaa-134">контейнер</span><span class="sxs-lookup"><span data-stu-id="efeaa-134">container</span></span>|[<span data-ttu-id="efeaa-135">plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="efeaa-135">plannerPlanContainer</span></span>](../resources/plannerplancontainer.md)|<span data-ttu-id="efeaa-136">Определяет контейнер плана.</span><span class="sxs-lookup"><span data-stu-id="efeaa-136">Identifies the container of the plan.</span></span> <span data-ttu-id="efeaa-137">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="efeaa-137">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="efeaa-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efeaa-138">Required.</span></span>|
|<span data-ttu-id="efeaa-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efeaa-139">createdDateTime</span></span>|<span data-ttu-id="efeaa-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efeaa-140">DateTimeOffset</span></span>|<span data-ttu-id="efeaa-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-141">Read-only.</span></span> <span data-ttu-id="efeaa-142">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="efeaa-142">Date and time at which the plan is created.</span></span> <span data-ttu-id="efeaa-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="efeaa-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="efeaa-144">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="efeaa-144">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="efeaa-145">id</span><span class="sxs-lookup"><span data-stu-id="efeaa-145">id</span></span>|<span data-ttu-id="efeaa-146">String</span><span class="sxs-lookup"><span data-stu-id="efeaa-146">String</span></span>| <span data-ttu-id="efeaa-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-147">Read-only.</span></span> <span data-ttu-id="efeaa-148">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="efeaa-148">ID of the plan.</span></span> <span data-ttu-id="efeaa-149">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="efeaa-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="efeaa-150">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="efeaa-150">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="efeaa-151">title</span><span class="sxs-lookup"><span data-stu-id="efeaa-151">title</span></span>|<span data-ttu-id="efeaa-152">String</span><span class="sxs-lookup"><span data-stu-id="efeaa-152">String</span></span>|<span data-ttu-id="efeaa-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efeaa-153">Required.</span></span> <span data-ttu-id="efeaa-154">Название плана.</span><span class="sxs-lookup"><span data-stu-id="efeaa-154">Title of the plan.</span></span>|
|<span data-ttu-id="efeaa-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="efeaa-155">createdBy</span></span>|[<span data-ttu-id="efeaa-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="efeaa-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="efeaa-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-157">Read-only.</span></span> <span data-ttu-id="efeaa-158">Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="efeaa-158">The user who created the plan.</span></span>|
|<span data-ttu-id="efeaa-159">контексты</span><span class="sxs-lookup"><span data-stu-id="efeaa-159">contexts</span></span>|<span data-ttu-id="efeaa-160">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="efeaa-160">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="efeaa-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-161">Read-only.</span></span> <span data-ttu-id="efeaa-162">Дополнительные пользовательские интерфейсы, в которых используется этот план, представлены в качестве [записей plannerPlanContext.](plannerplancontext.md)</span><span class="sxs-lookup"><span data-stu-id="efeaa-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|
|<span data-ttu-id="efeaa-163">владелец (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="efeaa-163">owner (deprecated)</span></span> |<span data-ttu-id="efeaa-164">String</span><span class="sxs-lookup"><span data-stu-id="efeaa-164">String</span></span>| <span data-ttu-id="efeaa-165">Вместо этого **используйте свойство контейнера.**</span><span class="sxs-lookup"><span data-stu-id="efeaa-165">Use the **container** property instead.</span></span> <span data-ttu-id="efeaa-166">ID [группы,](group.md) которая владеет планом.</span><span class="sxs-lookup"><span data-stu-id="efeaa-166">ID of the [group](group.md) that owns the plan.</span></span> <span data-ttu-id="efeaa-167">После установки значения обновить это свойство невозможно.</span><span class="sxs-lookup"><span data-stu-id="efeaa-167">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="efeaa-168">Это свойство не возвращает допустимый групповой ID, если контейнер плана не является группой.</span><span class="sxs-lookup"><span data-stu-id="efeaa-168">This property will not return a valid group ID if the container of the plan is not a group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efeaa-169">Связи</span><span class="sxs-lookup"><span data-stu-id="efeaa-169">Relationships</span></span>
| <span data-ttu-id="efeaa-170">Связь</span><span class="sxs-lookup"><span data-stu-id="efeaa-170">Relationship</span></span> | <span data-ttu-id="efeaa-171">Тип</span><span class="sxs-lookup"><span data-stu-id="efeaa-171">Type</span></span>   |<span data-ttu-id="efeaa-172">Описание</span><span class="sxs-lookup"><span data-stu-id="efeaa-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efeaa-173">buckets</span><span class="sxs-lookup"><span data-stu-id="efeaa-173">buckets</span></span>|<span data-ttu-id="efeaa-174">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="efeaa-174">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="efeaa-175">Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="efeaa-175">Collection of buckets in the plan.</span></span> <span data-ttu-id="efeaa-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-176">Read-only.</span></span> <span data-ttu-id="efeaa-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="efeaa-177">Nullable.</span></span>|
|<span data-ttu-id="efeaa-178">details</span><span class="sxs-lookup"><span data-stu-id="efeaa-178">details</span></span>|[<span data-ttu-id="efeaa-179">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="efeaa-179">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="efeaa-180">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="efeaa-180">Additional details about the plan.</span></span> <span data-ttu-id="efeaa-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-181">Read-only.</span></span> <span data-ttu-id="efeaa-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="efeaa-182">Nullable.</span></span> |
|<span data-ttu-id="efeaa-183">tasks</span><span class="sxs-lookup"><span data-stu-id="efeaa-183">tasks</span></span>|<span data-ttu-id="efeaa-184">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="efeaa-184">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="efeaa-185">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="efeaa-185">Collection of tasks in the plan.</span></span> <span data-ttu-id="efeaa-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efeaa-186">Read-only.</span></span> <span data-ttu-id="efeaa-187">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="efeaa-187">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="efeaa-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efeaa-188">JSON representation</span></span>

<span data-ttu-id="efeaa-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efeaa-189">Here is a JSON representation of the resource.</span></span>

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
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "String",
    "containerId": "String",
    "type": "String"
  },
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


