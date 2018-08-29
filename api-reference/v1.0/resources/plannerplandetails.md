# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="b412e-101">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b412e-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="b412e-p101">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="b412e-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="b412e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="b412e-104">Methods</span></span>

| <span data-ttu-id="b412e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="b412e-105">Method</span></span>           | <span data-ttu-id="b412e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b412e-106">Return Type</span></span>    |<span data-ttu-id="b412e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b412e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b412e-108">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b412e-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="b412e-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b412e-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="b412e-110">Чтение свойств и отношений объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="b412e-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="b412e-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="b412e-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="b412e-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b412e-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="b412e-113">Обновление объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="b412e-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b412e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="b412e-114">Properties</span></span>
| <span data-ttu-id="b412e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="b412e-115">Property</span></span>     | <span data-ttu-id="b412e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="b412e-116">Type</span></span>   |<span data-ttu-id="b412e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="b412e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b412e-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="b412e-118">categoryDescriptions</span></span>|[<span data-ttu-id="b412e-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="b412e-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="b412e-120">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="b412e-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="b412e-121">id</span><span class="sxs-lookup"><span data-stu-id="b412e-121">id</span></span>|<span data-ttu-id="b412e-122">строка</span><span class="sxs-lookup"><span data-stu-id="b412e-122">String</span></span>| <span data-ttu-id="b412e-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b412e-123">Read-only.</span></span> <span data-ttu-id="b412e-124">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="b412e-124">ID of the plan details.</span></span> <span data-ttu-id="b412e-125">Длина — 28 символов с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="b412e-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b412e-126">[Проверка формата](planner_identifiers_disclaimer.md) выполняется на службе.</span><span class="sxs-lookup"><span data-stu-id="b412e-126">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b412e-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="b412e-127">sharedWith</span></span>|[<span data-ttu-id="b412e-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="b412e-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="b412e-p103">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="b412e-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b412e-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b412e-132">Relationships</span></span>
<span data-ttu-id="b412e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b412e-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b412e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b412e-134">JSON representation</span></span>
<span data-ttu-id="b412e-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b412e-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->