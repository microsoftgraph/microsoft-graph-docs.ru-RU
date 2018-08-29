# <a name="planneruser-resource-type"></a><span data-ttu-id="ee7dc-101">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="ee7dc-101">plannerUser resource type</span></span>

<span data-ttu-id="ee7dc-p101">Ресурс **plannerUser** предоставляют доступ к ресурсам Планировщика для [пользователя](user.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-p101">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ee7dc-104">Методы</span><span class="sxs-lookup"><span data-stu-id="ee7dc-104">Methods</span></span>

| <span data-ttu-id="ee7dc-105">Метод</span><span class="sxs-lookup"><span data-stu-id="ee7dc-105">Method</span></span>           | <span data-ttu-id="ee7dc-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee7dc-106">Return Type</span></span>    |<span data-ttu-id="ee7dc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7dc-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee7dc-108">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="ee7dc-108">List plans</span></span>](../api/planneruser_list_plans.md) |<span data-ttu-id="ee7dc-109">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ee7dc-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ee7dc-110">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-110">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="ee7dc-111">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="ee7dc-111">List tasks</span></span>](../api/planneruser_list_tasks.md) |<span data-ttu-id="ee7dc-112">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ee7dc-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ee7dc-113">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-113">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee7dc-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee7dc-114">Properties</span></span>
| <span data-ttu-id="ee7dc-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee7dc-115">Property</span></span>     | <span data-ttu-id="ee7dc-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7dc-116">Type</span></span>   |<span data-ttu-id="ee7dc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7dc-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee7dc-118">id</span><span class="sxs-lookup"><span data-stu-id="ee7dc-118">id</span></span>|<span data-ttu-id="ee7dc-119">Cтрока</span><span class="sxs-lookup"><span data-stu-id="ee7dc-119">String</span></span>| <span data-ttu-id="ee7dc-p102">Только для чтения. Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="ee7dc-p102">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee7dc-122">Связи</span><span class="sxs-lookup"><span data-stu-id="ee7dc-122">Relationships</span></span>
| <span data-ttu-id="ee7dc-123">Связь</span><span class="sxs-lookup"><span data-stu-id="ee7dc-123">Relationship</span></span> | <span data-ttu-id="ee7dc-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7dc-124">Type</span></span>   |<span data-ttu-id="ee7dc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7dc-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee7dc-126">plans</span><span class="sxs-lookup"><span data-stu-id="ee7dc-126">plans</span></span>|<span data-ttu-id="ee7dc-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ee7dc-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ee7dc-p103">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="ee7dc-131">tasks</span><span class="sxs-lookup"><span data-stu-id="ee7dc-131">tasks</span></span>|<span data-ttu-id="ee7dc-132">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ee7dc-132">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ee7dc-p104">Только для чтения. Допускает значение null. Возвращает объекты [plannerPlan](plannerplan.md), к которым у пользователя есть доступ.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee7dc-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ee7dc-136">JSON representation</span></span>
<span data-ttu-id="ee7dc-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee7dc-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->