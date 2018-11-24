# <a name="plannerplan-resource-type"></a><span data-ttu-id="d2be1-101">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d2be1-101">plannerPlan resource type</span></span>

<span data-ttu-id="d2be1-p101">Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannerTask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerBucket.md). Каждый объект plan имеет объект [details](plannerPlanDetails.md), который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner_overview.md).</span><span class="sxs-lookup"><span data-stu-id="d2be1-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2be1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d2be1-107">Methods</span></span>

| <span data-ttu-id="d2be1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d2be1-108">Method</span></span>           | <span data-ttu-id="d2be1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2be1-109">Return Type</span></span>    |<span data-ttu-id="d2be1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2be1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2be1-111">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d2be1-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | <span data-ttu-id="d2be1-112">[plannerPlan](plannerplan.md);</span><span class="sxs-lookup"><span data-stu-id="d2be1-112">[plannerPlan](plannerplan.md)</span></span> |<span data-ttu-id="d2be1-113">Считывание свойств и связей объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d2be1-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="d2be1-114">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="d2be1-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="d2be1-115">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d2be1-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d2be1-116">Получение коллекции объектов **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="d2be1-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="d2be1-117">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="d2be1-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="d2be1-118">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d2be1-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d2be1-119">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="d2be1-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="d2be1-120">Update</span><span class="sxs-lookup"><span data-stu-id="d2be1-120">Update</span></span>](../api/plannerplan_update.md) | <span data-ttu-id="d2be1-121">[plannerPlan](plannerplan.md);</span><span class="sxs-lookup"><span data-stu-id="d2be1-121">[plannerPlan](plannerplan.md)</span></span> |<span data-ttu-id="d2be1-122">Обновление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d2be1-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2be1-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2be1-123">Properties</span></span>
| <span data-ttu-id="d2be1-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2be1-124">Property</span></span>     | <span data-ttu-id="d2be1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d2be1-125">Type</span></span>   |<span data-ttu-id="d2be1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d2be1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2be1-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2be1-127">createdDateTime</span></span>|<span data-ttu-id="d2be1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2be1-128">DateTimeOffset</span></span>|<span data-ttu-id="d2be1-p102">Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d2be1-133">id</span><span class="sxs-lookup"><span data-stu-id="d2be1-133">id</span></span>|<span data-ttu-id="d2be1-134">String</span><span class="sxs-lookup"><span data-stu-id="d2be1-134">String</span></span>| <span data-ttu-id="d2be1-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2be1-135">Read-only.</span></span> <span data-ttu-id="d2be1-136">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="d2be1-136">ID of the plan.</span></span> <span data-ttu-id="d2be1-137">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d2be1-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d2be1-138">[Формат](planner_identifiers_disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="d2be1-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d2be1-139">owner</span><span class="sxs-lookup"><span data-stu-id="d2be1-139">owner</span></span>|<span data-ttu-id="d2be1-140">String</span><span class="sxs-lookup"><span data-stu-id="d2be1-140">String</span></span>|<span data-ttu-id="d2be1-141">Идентификатор [группы](group.md) , который несет ответственность за планирование.</span><span class="sxs-lookup"><span data-stu-id="d2be1-141">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="d2be1-142">В этом поле можно указать допустимое группы должен существовать.</span><span class="sxs-lookup"><span data-stu-id="d2be1-142">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="d2be1-143">После его установки, это свойство не удается обновить.</span><span class="sxs-lookup"><span data-stu-id="d2be1-143">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="d2be1-144">title</span><span class="sxs-lookup"><span data-stu-id="d2be1-144">title</span></span>|<span data-ttu-id="d2be1-145">String</span><span class="sxs-lookup"><span data-stu-id="d2be1-145">String</span></span>|<span data-ttu-id="d2be1-p105">Обязательный. Название плана.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="d2be1-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="d2be1-148">createdBy</span></span>|[<span data-ttu-id="d2be1-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="d2be1-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="d2be1-p106">Только для чтения. Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2be1-152">Связи</span><span class="sxs-lookup"><span data-stu-id="d2be1-152">Relationships</span></span>
| <span data-ttu-id="d2be1-153">Связь</span><span class="sxs-lookup"><span data-stu-id="d2be1-153">Relationship</span></span> | <span data-ttu-id="d2be1-154">Тип</span><span class="sxs-lookup"><span data-stu-id="d2be1-154">Type</span></span>   |<span data-ttu-id="d2be1-155">Описание</span><span class="sxs-lookup"><span data-stu-id="d2be1-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2be1-156">buckets</span><span class="sxs-lookup"><span data-stu-id="d2be1-156">buckets</span></span>|<span data-ttu-id="d2be1-157">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d2be1-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d2be1-p107">Только для чтения. Допускает значение null. Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="d2be1-161">details</span><span class="sxs-lookup"><span data-stu-id="d2be1-161">details</span></span>|<span data-ttu-id="d2be1-162">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="d2be1-162">[plannerPlanDetails](plannerplandetails.md)</span></span>| <span data-ttu-id="d2be1-p108">Только для чтения. Допускает значение null. Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="d2be1-166">tasks</span><span class="sxs-lookup"><span data-stu-id="d2be1-166">tasks</span></span>|<span data-ttu-id="d2be1-167">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d2be1-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d2be1-p109">Только для чтения. Допускает значение null. Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="d2be1-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2be1-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2be1-171">JSON representation</span></span>

<span data-ttu-id="d2be1-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2be1-172">Here is a JSON representation of the resource.</span></span>

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