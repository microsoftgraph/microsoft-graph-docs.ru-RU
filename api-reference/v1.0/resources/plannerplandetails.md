# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="26ccf-101">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="26ccf-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="26ccf-p101">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="26ccf-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="26ccf-104">Методы</span><span class="sxs-lookup"><span data-stu-id="26ccf-104">Methods</span></span>

| <span data-ttu-id="26ccf-105">Метод</span><span class="sxs-lookup"><span data-stu-id="26ccf-105">Method</span></span>           | <span data-ttu-id="26ccf-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26ccf-106">Return Type</span></span>    |<span data-ttu-id="26ccf-107">Описание</span><span class="sxs-lookup"><span data-stu-id="26ccf-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26ccf-108">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="26ccf-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="26ccf-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="26ccf-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="26ccf-110">Чтение свойств и отношений объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="26ccf-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="26ccf-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="26ccf-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="26ccf-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="26ccf-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="26ccf-113">Обновление объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="26ccf-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="26ccf-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="26ccf-114">Properties</span></span>
| <span data-ttu-id="26ccf-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="26ccf-115">Property</span></span>     | <span data-ttu-id="26ccf-116">Тип</span><span class="sxs-lookup"><span data-stu-id="26ccf-116">Type</span></span>   |<span data-ttu-id="26ccf-117">Описание</span><span class="sxs-lookup"><span data-stu-id="26ccf-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26ccf-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="26ccf-118">categoryDescriptions</span></span>|[<span data-ttu-id="26ccf-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="26ccf-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="26ccf-120">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="26ccf-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="26ccf-121">id</span><span class="sxs-lookup"><span data-stu-id="26ccf-121">id</span></span>|<span data-ttu-id="26ccf-122">String</span><span class="sxs-lookup"><span data-stu-id="26ccf-122">String</span></span>| <span data-ttu-id="26ccf-p102">Только для чтения. Идентификатор сведений о плане. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](planner_identifiers_disclaimer.md) выполняется для службы.</span><span class="sxs-lookup"><span data-stu-id="26ccf-p102">Read-only. ID of the plan details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="26ccf-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="26ccf-127">sharedWith</span></span>|[<span data-ttu-id="26ccf-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="26ccf-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="26ccf-p103">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="26ccf-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="26ccf-132">Связи</span><span class="sxs-lookup"><span data-stu-id="26ccf-132">Relationships</span></span>
<span data-ttu-id="26ccf-133">Нет</span><span class="sxs-lookup"><span data-stu-id="26ccf-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="26ccf-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26ccf-134">JSON representation</span></span>
<span data-ttu-id="26ccf-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26ccf-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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