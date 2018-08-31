# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="5e678-101">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="5e678-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="5e678-p101">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="5e678-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="5e678-104">Методы</span><span class="sxs-lookup"><span data-stu-id="5e678-104">Methods</span></span>

| <span data-ttu-id="5e678-105">Метод</span><span class="sxs-lookup"><span data-stu-id="5e678-105">Method</span></span>           | <span data-ttu-id="5e678-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e678-106">Return Type</span></span>    |<span data-ttu-id="5e678-107">Описание</span><span class="sxs-lookup"><span data-stu-id="5e678-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e678-108">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="5e678-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="5e678-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="5e678-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="5e678-110">Чтение свойств и отношений объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="5e678-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="5e678-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="5e678-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="5e678-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="5e678-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="5e678-113">Обновление объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="5e678-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e678-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e678-114">Properties</span></span>
| <span data-ttu-id="5e678-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e678-115">Property</span></span>     | <span data-ttu-id="5e678-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5e678-116">Type</span></span>   |<span data-ttu-id="5e678-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5e678-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e678-118">checklist</span><span class="sxs-lookup"><span data-stu-id="5e678-118">checklist</span></span>|[<span data-ttu-id="5e678-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="5e678-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="5e678-120">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="5e678-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="5e678-121">description</span><span class="sxs-lookup"><span data-stu-id="5e678-121">description</span></span>|<span data-ttu-id="5e678-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5e678-122">String</span></span>|<span data-ttu-id="5e678-123">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="5e678-123">Description of the task</span></span>|
|<span data-ttu-id="5e678-124">id</span><span class="sxs-lookup"><span data-stu-id="5e678-124">id</span></span>|<span data-ttu-id="5e678-125">строка</span><span class="sxs-lookup"><span data-stu-id="5e678-125">String</span></span>| <span data-ttu-id="5e678-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e678-126">Read-only.</span></span> <span data-ttu-id="5e678-127">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="5e678-127">ID of the task details.</span></span> <span data-ttu-id="5e678-128">Длина — 28 знаков с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="5e678-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5e678-129">[Проверка формата](planner_identifiers_disclaimer.md) выполняется с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="5e678-129">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5e678-130">previewType</span><span class="sxs-lookup"><span data-stu-id="5e678-130">previewType</span></span>|<span data-ttu-id="5e678-131">string</span><span class="sxs-lookup"><span data-stu-id="5e678-131">string</span></span>|<span data-ttu-id="5e678-132">Задает тип предварительной версии, которая отображается на задаче.</span><span class="sxs-lookup"><span data-stu-id="5e678-132">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="5e678-133">Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="5e678-133">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="5e678-134">Если параметр имеет значение `automatic`, отображаемая версия предварительного просмотра выбирается приложением просмотра задачи.</span><span class="sxs-lookup"><span data-stu-id="5e678-134">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="5e678-135">references</span><span class="sxs-lookup"><span data-stu-id="5e678-135">references</span></span>|[<span data-ttu-id="5e678-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="5e678-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="5e678-137">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="5e678-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e678-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e678-138">Relationships</span></span>
<span data-ttu-id="5e678-139">Нет</span><span class="sxs-lookup"><span data-stu-id="5e678-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e678-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e678-140">JSON representation</span></span>
<span data-ttu-id="5e678-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e678-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
