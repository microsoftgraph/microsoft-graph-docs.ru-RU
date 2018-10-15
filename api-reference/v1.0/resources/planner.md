# <a name="planner-resource-type"></a><span data-ttu-id="3cff5-101">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="3cff5-101">planner resource type</span></span>

<span data-ttu-id="3cff5-p101">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="3cff5-p101">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="3cff5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3cff5-105">Methods</span></span>

| <span data-ttu-id="3cff5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3cff5-106">Method</span></span>           | <span data-ttu-id="3cff5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3cff5-107">Return Type</span></span>    |<span data-ttu-id="3cff5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3cff5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3cff5-109">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3cff5-109">Create plannerBucket</span></span>](../api/planner_post_buckets.md) |[<span data-ttu-id="3cff5-110">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3cff5-110">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="3cff5-111">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="3cff5-111">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="3cff5-112">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3cff5-112">Create plannerPlan</span></span>](../api/planner_post_plans.md) |[<span data-ttu-id="3cff5-113">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3cff5-113">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="3cff5-114">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="3cff5-114">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="3cff5-115">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="3cff5-115">Create plannerTask</span></span>](../api/planner_post_tasks.md) |[<span data-ttu-id="3cff5-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="3cff5-116">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="3cff5-117">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="3cff5-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cff5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3cff5-118">Relationships</span></span>
| <span data-ttu-id="3cff5-119">Связь</span><span class="sxs-lookup"><span data-stu-id="3cff5-119">Relationship</span></span> | <span data-ttu-id="3cff5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3cff5-120">Type</span></span>   |<span data-ttu-id="3cff5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3cff5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cff5-122">buckets</span><span class="sxs-lookup"><span data-stu-id="3cff5-122">buckets</span></span>|<span data-ttu-id="3cff5-123">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="3cff5-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="3cff5-p102">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="3cff5-p102">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="3cff5-127">plans</span><span class="sxs-lookup"><span data-stu-id="3cff5-127">plans</span></span>|<span data-ttu-id="3cff5-128">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3cff5-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3cff5-p103">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="3cff5-p103">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="3cff5-132">tasks</span><span class="sxs-lookup"><span data-stu-id="3cff5-132">tasks</span></span>|<span data-ttu-id="3cff5-133">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="3cff5-133">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3cff5-p104">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="3cff5-p104">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cff5-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3cff5-137">JSON representation</span></span>
<span data-ttu-id="3cff5-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cff5-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="3cff5-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3cff5-139">Example</span></span>

<span data-ttu-id="3cff5-140">Ресурс **planner** доступен в корне диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3cff5-140">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->