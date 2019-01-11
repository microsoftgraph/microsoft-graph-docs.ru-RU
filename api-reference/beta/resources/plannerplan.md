---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержит коллекцию plannerTasks. Он также может иметь коллекцию plannerBuckets. Каждый объект плана имеет сведения о объекта, которое может содержать дополнительные сведения о плане. Дополнительные сведения о связях между группами, планы и задачи можно планировщик работы.
localization_priority: Normal
ms.openlocfilehash: 4890daa6ad221a36cf0029b49ce39560fc80afcd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888104"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="396a3-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="396a3-107">plannerPlan resource type</span></span>

> <span data-ttu-id="396a3-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="396a3-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="396a3-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="396a3-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="396a3-110">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="396a3-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="396a3-111">План может принадлежать [группе](group.md) и содержит коллекцию [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="396a3-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="396a3-112">Он также может иметь коллекцию [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="396a3-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="396a3-113">Каждый объект плана имеет [сведения о](plannerplandetails.md) объекта, которое может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="396a3-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="396a3-114">Дополнительные сведения о связях между группами, планы и задачи можно [Планировщик работы](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="396a3-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="396a3-115">Методы</span><span class="sxs-lookup"><span data-stu-id="396a3-115">Methods</span></span>

| <span data-ttu-id="396a3-116">Метод</span><span class="sxs-lookup"><span data-stu-id="396a3-116">Method</span></span>           | <span data-ttu-id="396a3-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="396a3-117">Return Type</span></span>    |<span data-ttu-id="396a3-118">Описание</span><span class="sxs-lookup"><span data-stu-id="396a3-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="396a3-119">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="396a3-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="396a3-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="396a3-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="396a3-121">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="396a3-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="396a3-122">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="396a3-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="396a3-123">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="396a3-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="396a3-124">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="396a3-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="396a3-125">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="396a3-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="396a3-126">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="396a3-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="396a3-127">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="396a3-127">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="396a3-128">[обновление](../api/plannerplan-update.md).</span><span class="sxs-lookup"><span data-stu-id="396a3-128">[Update](../api/plannerplan-update.md)</span></span> | [<span data-ttu-id="396a3-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="396a3-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="396a3-130">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="396a3-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="396a3-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="396a3-131">Properties</span></span>
| <span data-ttu-id="396a3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="396a3-132">Property</span></span>     | <span data-ttu-id="396a3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="396a3-133">Type</span></span>   |<span data-ttu-id="396a3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="396a3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="396a3-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="396a3-135">createdDateTime</span></span>|<span data-ttu-id="396a3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="396a3-136">DateTimeOffset</span></span>|<span data-ttu-id="396a3-p104">Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="396a3-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="396a3-141">id</span><span class="sxs-lookup"><span data-stu-id="396a3-141">id</span></span>|<span data-ttu-id="396a3-142">Строка</span><span class="sxs-lookup"><span data-stu-id="396a3-142">String</span></span>| <span data-ttu-id="396a3-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="396a3-143">Read-only.</span></span> <span data-ttu-id="396a3-144">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="396a3-144">ID of the plan.</span></span> <span data-ttu-id="396a3-145">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="396a3-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="396a3-146">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="396a3-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="396a3-147">owner</span><span class="sxs-lookup"><span data-stu-id="396a3-147">owner</span></span>|<span data-ttu-id="396a3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="396a3-148">String</span></span>|<span data-ttu-id="396a3-149">Идентификатор [группы](group.md) , который несет ответственность за планирование.</span><span class="sxs-lookup"><span data-stu-id="396a3-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="396a3-150">В этом поле можно указать допустимое группы должен существовать.</span><span class="sxs-lookup"><span data-stu-id="396a3-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="396a3-151">После его установки, это свойство не удается обновить.</span><span class="sxs-lookup"><span data-stu-id="396a3-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="396a3-152">title</span><span class="sxs-lookup"><span data-stu-id="396a3-152">title</span></span>|<span data-ttu-id="396a3-153">String</span><span class="sxs-lookup"><span data-stu-id="396a3-153">String</span></span>|<span data-ttu-id="396a3-p107">Обязательный. Название плана.</span><span class="sxs-lookup"><span data-stu-id="396a3-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="396a3-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="396a3-156">createdBy</span></span>|[<span data-ttu-id="396a3-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="396a3-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="396a3-p108">Только для чтения. Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="396a3-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="396a3-160">контекстов</span><span class="sxs-lookup"><span data-stu-id="396a3-160">contexts</span></span>|<span data-ttu-id="396a3-161">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="396a3-161">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="396a3-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="396a3-162">Read-only.</span></span> <span data-ttu-id="396a3-163">Дополнительные пользовательских интерфейсов, в которых используется этот план, представленные в виде [plannerPlanContext](plannerplancontext.md) записей.</span><span class="sxs-lookup"><span data-stu-id="396a3-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="396a3-164">Связи</span><span class="sxs-lookup"><span data-stu-id="396a3-164">Relationships</span></span>
| <span data-ttu-id="396a3-165">Связь</span><span class="sxs-lookup"><span data-stu-id="396a3-165">Relationship</span></span> | <span data-ttu-id="396a3-166">Тип</span><span class="sxs-lookup"><span data-stu-id="396a3-166">Type</span></span>   |<span data-ttu-id="396a3-167">Описание</span><span class="sxs-lookup"><span data-stu-id="396a3-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="396a3-168">buckets</span><span class="sxs-lookup"><span data-stu-id="396a3-168">buckets</span></span>|<span data-ttu-id="396a3-169">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="396a3-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="396a3-p110">Только для чтения. Допускает значение null. Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="396a3-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="396a3-173">details</span><span class="sxs-lookup"><span data-stu-id="396a3-173">details</span></span>|<span data-ttu-id="396a3-174">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="396a3-174">[plannerPlanDetails](plannerplandetails.md)</span></span>| <span data-ttu-id="396a3-p111">Только для чтения. Допускает значение null. Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="396a3-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="396a3-178">tasks</span><span class="sxs-lookup"><span data-stu-id="396a3-178">tasks</span></span>|<span data-ttu-id="396a3-179">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="396a3-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="396a3-p112">Только для чтения. Допускает значение null. Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="396a3-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="396a3-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="396a3-183">JSON representation</span></span>

<span data-ttu-id="396a3-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="396a3-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
