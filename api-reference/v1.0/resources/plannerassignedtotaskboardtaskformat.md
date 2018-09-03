# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="9b3c7-101">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9b3c7-101">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="9b3c7-p101">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-p101">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="9b3c7-104">Методы</span><span class="sxs-lookup"><span data-stu-id="9b3c7-104">Methods</span></span>

| <span data-ttu-id="9b3c7-105">Метод</span><span class="sxs-lookup"><span data-stu-id="9b3c7-105">Method</span></span>           | <span data-ttu-id="9b3c7-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b3c7-106">Return Type</span></span>    |<span data-ttu-id="9b3c7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9b3c7-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b3c7-108">Получение plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9b3c7-108">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat_get.md) | [<span data-ttu-id="9b3c7-109">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9b3c7-109">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="9b3c7-110">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-110">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="9b3c7-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="9b3c7-111">Update</span></span>](../api/plannerassignedtotaskboardtaskformat_update.md) | [<span data-ttu-id="9b3c7-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9b3c7-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="9b3c7-113">Обновление объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-113">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b3c7-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b3c7-114">Properties</span></span>
| <span data-ttu-id="9b3c7-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b3c7-115">Property</span></span>     | <span data-ttu-id="9b3c7-116">Тип</span><span class="sxs-lookup"><span data-stu-id="9b3c7-116">Type</span></span>   |<span data-ttu-id="9b3c7-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9b3c7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b3c7-118">id</span><span class="sxs-lookup"><span data-stu-id="9b3c7-118">id</span></span>|<span data-ttu-id="9b3c7-119">строка</span><span class="sxs-lookup"><span data-stu-id="9b3c7-119">String</span></span>| <span data-ttu-id="9b3c7-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-120">Read-only.</span></span> <span data-ttu-id="9b3c7-121">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-121">The ID of the resource.</span></span> <span data-ttu-id="9b3c7-122">Длина — 28 знаков с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9b3c7-123">[Проверка формата](planner_identifiers_disclaimer.md) выполняется с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9b3c7-124">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9b3c7-124">orderHintsByAssignee</span></span>|[<span data-ttu-id="9b3c7-125">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9b3c7-125">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="9b3c7-p103">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="9b3c7-p103">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="9b3c7-129">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="9b3c7-129">unassignedOrderHint</span></span>|<span data-ttu-id="9b3c7-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9b3c7-130">String</span></span>|<span data-ttu-id="9b3c7-p104">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="9b3c7-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b3c7-133">Связи</span><span class="sxs-lookup"><span data-stu-id="9b3c7-133">Relationships</span></span>
<span data-ttu-id="9b3c7-134">Нет</span><span class="sxs-lookup"><span data-stu-id="9b3c7-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b3c7-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b3c7-135">JSON representation</span></span>
<span data-ttu-id="9b3c7-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b3c7-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->