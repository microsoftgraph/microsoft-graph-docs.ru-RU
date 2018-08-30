# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="da339-101">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da339-101">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="da339-p101">Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="da339-p101">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="da339-104">Методы</span><span class="sxs-lookup"><span data-stu-id="da339-104">Methods</span></span>

| <span data-ttu-id="da339-105">Метод</span><span class="sxs-lookup"><span data-stu-id="da339-105">Method</span></span>           | <span data-ttu-id="da339-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da339-106">Return Type</span></span>    |<span data-ttu-id="da339-107">Описание</span><span class="sxs-lookup"><span data-stu-id="da339-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da339-108">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da339-108">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat_get.md) | [<span data-ttu-id="da339-109">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da339-109">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="da339-110">Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="da339-110">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="da339-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="da339-111">Update</span></span>](../api/plannerprogresstaskboardtaskformat_update.md) | [<span data-ttu-id="da339-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da339-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="da339-113">Обновление объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="da339-113">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="da339-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="da339-114">Properties</span></span>
| <span data-ttu-id="da339-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="da339-115">Property</span></span>     | <span data-ttu-id="da339-116">Тип</span><span class="sxs-lookup"><span data-stu-id="da339-116">Type</span></span>   |<span data-ttu-id="da339-117">Описание</span><span class="sxs-lookup"><span data-stu-id="da339-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da339-118">id</span><span class="sxs-lookup"><span data-stu-id="da339-118">id</span></span>|<span data-ttu-id="da339-119">Строка​</span><span class="sxs-lookup"><span data-stu-id="da339-119">String</span></span>| <span data-ttu-id="da339-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da339-120">Read-only.</span></span> <span data-ttu-id="da339-121">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="da339-121">The ID of the resource.</span></span> <span data-ttu-id="da339-122">Длина — 28 символов с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="da339-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="da339-123">[Проверка формата](planner_identifiers_disclaimer.md) выполняется на службе.</span><span class="sxs-lookup"><span data-stu-id="da339-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="da339-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="da339-124">orderHint</span></span>|<span data-ttu-id="da339-125">Строка​</span><span class="sxs-lookup"><span data-stu-id="da339-125">String</span></span>|<span data-ttu-id="da339-p103">Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="da339-p103">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="da339-128">Связи</span><span class="sxs-lookup"><span data-stu-id="da339-128">Relationships</span></span>
<span data-ttu-id="da339-129">Нет</span><span class="sxs-lookup"><span data-stu-id="da339-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="da339-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da339-130">JSON representation</span></span>
<span data-ttu-id="da339-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da339-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->