# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="be063-101">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="be063-101">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="be063-p101">Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом [task](plannertask.md) связан один объект **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="be063-p101">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="be063-104">Методы</span><span class="sxs-lookup"><span data-stu-id="be063-104">Methods</span></span>

| <span data-ttu-id="be063-105">Метод</span><span class="sxs-lookup"><span data-stu-id="be063-105">Method</span></span>           | <span data-ttu-id="be063-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be063-106">Return Type</span></span>    |<span data-ttu-id="be063-107">Описание</span><span class="sxs-lookup"><span data-stu-id="be063-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be063-108">Получение plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="be063-108">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat_get.md) | [<span data-ttu-id="be063-109">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="be063-109">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="be063-110">Считывание свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="be063-110">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="be063-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="be063-111">Update</span></span>](../api/plannerbuckettaskboardtaskformat_update.md) | [<span data-ttu-id="be063-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="be063-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="be063-113">Обновление объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="be063-113">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be063-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="be063-114">Properties</span></span>
| <span data-ttu-id="be063-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="be063-115">Property</span></span>     | <span data-ttu-id="be063-116">Тип</span><span class="sxs-lookup"><span data-stu-id="be063-116">Type</span></span>   |<span data-ttu-id="be063-117">Описание</span><span class="sxs-lookup"><span data-stu-id="be063-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be063-118">id</span><span class="sxs-lookup"><span data-stu-id="be063-118">id</span></span>|<span data-ttu-id="be063-119">Строка</span><span class="sxs-lookup"><span data-stu-id="be063-119">String</span></span>| <span data-ttu-id="be063-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be063-120">Read-only.</span></span> <span data-ttu-id="be063-121">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="be063-121">The ID of the resource.</span></span> <span data-ttu-id="be063-122">Длина — 28 знаков с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="be063-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="be063-123">[Проверка формата](planner_identifiers_disclaimer.md) выполняется на службе.</span><span class="sxs-lookup"><span data-stu-id="be063-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="be063-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="be063-124">orderHint</span></span>|<span data-ttu-id="be063-125">Строка</span><span class="sxs-lookup"><span data-stu-id="be063-125">String</span></span>|<span data-ttu-id="be063-p103">Указание, используемое для расположения задач в представлении сегментов на доске задач. Используемый формат описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="be063-p103">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="be063-128">Связи</span><span class="sxs-lookup"><span data-stu-id="be063-128">Relationships</span></span>
<span data-ttu-id="be063-129">Нет</span><span class="sxs-lookup"><span data-stu-id="be063-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="be063-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be063-130">JSON representation</span></span>
<span data-ttu-id="be063-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be063-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->