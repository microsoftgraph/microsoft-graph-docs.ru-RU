# <a name="plannerbucket-resource-type"></a><span data-ttu-id="651b7-101">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="651b7-101">plannerBucket resource type</span></span>

<span data-ttu-id="651b7-p101">Ресурс **plannerBucket** представляет сегмент (или "специальный столбец") для задач плана в Office 365. Он содержится в объекте [plannerPlan](plannerPlan.md) и может содержать коллекцию объектов [plannerTasks](plannerTask.md).</span><span class="sxs-lookup"><span data-stu-id="651b7-p101">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerPlan.md) and can have a collection of [plannerTasks](plannerTask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="651b7-104">Методы</span><span class="sxs-lookup"><span data-stu-id="651b7-104">Methods</span></span>

| <span data-ttu-id="651b7-105">Метод</span><span class="sxs-lookup"><span data-stu-id="651b7-105">Method</span></span>           | <span data-ttu-id="651b7-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="651b7-106">Return Type</span></span>    |<span data-ttu-id="651b7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="651b7-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="651b7-108">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="651b7-108">Get plannerBucket</span></span>](../api/plannerbucket_get.md) | [<span data-ttu-id="651b7-109">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="651b7-109">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="651b7-110">Чтение свойств и отношений объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="651b7-110">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="651b7-111">Перечисление объектов plannerTasks</span><span class="sxs-lookup"><span data-stu-id="651b7-111">List plannerTasks</span></span>](../api/plannerbucket_list_tasks.md) |<span data-ttu-id="651b7-112">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="651b7-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="651b7-113">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="651b7-113">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="651b7-114">Создание</span><span class="sxs-lookup"><span data-stu-id="651b7-114">Create</span></span>](../api/planner_post_buckets.md) | [<span data-ttu-id="651b7-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="651b7-115">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="651b7-116">Создание объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="651b7-116">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="651b7-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="651b7-117">Update</span></span>](../api/plannerbucket_update.md) | [<span data-ttu-id="651b7-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="651b7-118">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="651b7-119">Обновление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="651b7-119">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="651b7-120">Удаление</span><span class="sxs-lookup"><span data-stu-id="651b7-120">Delete</span></span>](../api/plannerbucket_delete.md) | <span data-ttu-id="651b7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="651b7-121">None</span></span> |<span data-ttu-id="651b7-122">Удаление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="651b7-122">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="651b7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="651b7-123">Properties</span></span>
| <span data-ttu-id="651b7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="651b7-124">Property</span></span>     | <span data-ttu-id="651b7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="651b7-125">Type</span></span>   |<span data-ttu-id="651b7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="651b7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="651b7-127">id</span><span class="sxs-lookup"><span data-stu-id="651b7-127">id</span></span>|<span data-ttu-id="651b7-128">строка</span><span class="sxs-lookup"><span data-stu-id="651b7-128">String</span></span>| <span data-ttu-id="651b7-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="651b7-129">Read-only.</span></span> <span data-ttu-id="651b7-130">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="651b7-130">Name of the bucket.</span></span> <span data-ttu-id="651b7-131">Его длина — 28 символов с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="651b7-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="651b7-132">[Проверка формата](planner_identifiers_disclaimer.md) выполняется на службе.</span><span class="sxs-lookup"><span data-stu-id="651b7-132">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="651b7-133">name</span><span class="sxs-lookup"><span data-stu-id="651b7-133">name</span></span>|<span data-ttu-id="651b7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="651b7-134">String</span></span>|<span data-ttu-id="651b7-135">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="651b7-135">Name of the bucket.</span></span>|
|<span data-ttu-id="651b7-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="651b7-136">orderHint</span></span>|<span data-ttu-id="651b7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="651b7-137">String</span></span>|<span data-ttu-id="651b7-p103">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="651b7-p103">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="651b7-140">planId</span><span class="sxs-lookup"><span data-stu-id="651b7-140">planId</span></span>|<span data-ttu-id="651b7-141">Строка</span><span class="sxs-lookup"><span data-stu-id="651b7-141">String</span></span>|<span data-ttu-id="651b7-142">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="651b7-142">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="651b7-143">Связи</span><span class="sxs-lookup"><span data-stu-id="651b7-143">Relationships</span></span>
| <span data-ttu-id="651b7-144">Связь</span><span class="sxs-lookup"><span data-stu-id="651b7-144">Relationship</span></span> | <span data-ttu-id="651b7-145">Тип</span><span class="sxs-lookup"><span data-stu-id="651b7-145">Type</span></span>   |<span data-ttu-id="651b7-146">Описание</span><span class="sxs-lookup"><span data-stu-id="651b7-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="651b7-147">tasks</span><span class="sxs-lookup"><span data-stu-id="651b7-147">tasks</span></span>|<span data-ttu-id="651b7-148">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="651b7-148">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="651b7-p104">Только для чтения. Допускает значение null. Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="651b7-p104">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="651b7-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="651b7-152">JSON representation</span></span>
<span data-ttu-id="651b7-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="651b7-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->