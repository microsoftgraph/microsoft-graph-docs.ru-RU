# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="1ede4-101">Тип ресурса plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="1ede4-101">plannerAppliedCategories resource type</span></span>


<span data-ttu-id="1ede4-p101">Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или меток), примененных к задаче. Он является частью объекта [plannerTask](plannertask.md). К задаче можно применить до 6 категорий. Описания категорий, например `category1` и `category2`, являются частью объекта [сведений о плане](plannerplandetails.md). Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="1ede4-p101">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="1ede4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ede4-107">Properties</span></span>
<span data-ttu-id="1ede4-p102">Клиент может определять свойства открытого типа. В этом случае клиент должен указать значения для свойств `category1`, `category2`, `category3`, `category4`, `category5` или `category6`, а также использовать логическое значение `true` при применении соответствующих категорий к задаче. Ниже показан пример. Если не применить свойства, они будут автоматически удалены. Для этого им будет присвоено логическое значение `false`.</span><span class="sxs-lookup"><span data-stu-id="1ede4-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1ede4-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1ede4-112">JSON representation</span></span>

<span data-ttu-id="1ede4-113">Ниже показано представление ресурса в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1ede4-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="1ede4-114">Пример:</span><span class="sxs-lookup"><span data-stu-id="1ede4-114">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->