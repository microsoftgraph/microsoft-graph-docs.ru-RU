# <a name="plannergroup-resource-type"></a><span data-ttu-id="ff0b7-101">Тип ресурса plannerGroup</span><span class="sxs-lookup"><span data-stu-id="ff0b7-101">plannerGroup resource type</span></span>

<span data-ttu-id="ff0b7-p101">Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="ff0b7-p101">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ff0b7-104">Методы</span><span class="sxs-lookup"><span data-stu-id="ff0b7-104">Methods</span></span>

| <span data-ttu-id="ff0b7-105">Метод</span><span class="sxs-lookup"><span data-stu-id="ff0b7-105">Method</span></span>           | <span data-ttu-id="ff0b7-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff0b7-106">Return Type</span></span>    |<span data-ttu-id="ff0b7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0b7-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff0b7-108">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="ff0b7-108">List plans</span></span>](../api/plannergroup_list_plans.md) |<span data-ttu-id="ff0b7-109">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ff0b7-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ff0b7-110">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="ff0b7-110">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff0b7-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff0b7-111">Properties</span></span>
| <span data-ttu-id="ff0b7-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff0b7-112">Property</span></span>     | <span data-ttu-id="ff0b7-113">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0b7-113">Type</span></span>   |<span data-ttu-id="ff0b7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0b7-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0b7-115">id</span><span class="sxs-lookup"><span data-stu-id="ff0b7-115">id</span></span>|<span data-ttu-id="ff0b7-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ff0b7-116">String</span></span>| <span data-ttu-id="ff0b7-p102">Только для чтения. Идентификатор объекта **plannerGroup**.</span><span class="sxs-lookup"><span data-stu-id="ff0b7-p102">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0b7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ff0b7-119">Relationships</span></span>
| <span data-ttu-id="ff0b7-120">Связь</span><span class="sxs-lookup"><span data-stu-id="ff0b7-120">Relationship</span></span> | <span data-ttu-id="ff0b7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0b7-121">Type</span></span>   |<span data-ttu-id="ff0b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0b7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0b7-123">планы</span><span class="sxs-lookup"><span data-stu-id="ff0b7-123">plans</span></span>|<span data-ttu-id="ff0b7-124">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ff0b7-124">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ff0b7-p103">Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.</span><span class="sxs-lookup"><span data-stu-id="ff0b7-p103">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff0b7-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ff0b7-128">JSON representation</span></span>
<span data-ttu-id="ff0b7-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff0b7-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->