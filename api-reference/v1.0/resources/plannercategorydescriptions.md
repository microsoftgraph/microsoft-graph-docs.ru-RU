<span data-ttu-id="950f4-p101">Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="950f4-p101">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span>

Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий. 


## <span data-ttu-id="950f4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="950f4-105">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="950f4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="950f4-106">Property</span></span>     | <span data-ttu-id="950f4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="950f4-107">Type</span></span>   |<span data-ttu-id="950f4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="950f4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950f4-109">category1</span><span class="sxs-lookup"><span data-stu-id="950f4-109">category1</span></span>|<span data-ttu-id="950f4-110">String</span><span class="sxs-lookup"><span data-stu-id="950f4-110">String</span></span>|<span data-ttu-id="950f4-111">Метка, сопоставленная с категорией 1.</span><span class="sxs-lookup"><span data-stu-id="950f4-111">The label associated with Category 1</span></span>|
|<span data-ttu-id="950f4-112">category2</span><span class="sxs-lookup"><span data-stu-id="950f4-112">category2</span></span>|<span data-ttu-id="950f4-113">String</span><span class="sxs-lookup"><span data-stu-id="950f4-113">String</span></span>|<span data-ttu-id="950f4-114">Метка, сопоставленная с категорией 2.</span><span class="sxs-lookup"><span data-stu-id="950f4-114">The label associated with Category 2</span></span>|
|<span data-ttu-id="950f4-115">category3</span><span class="sxs-lookup"><span data-stu-id="950f4-115">category3</span></span>|<span data-ttu-id="950f4-116">String</span><span class="sxs-lookup"><span data-stu-id="950f4-116">String</span></span>|<span data-ttu-id="950f4-117">Метка, сопоставленная с категорией 3.</span><span class="sxs-lookup"><span data-stu-id="950f4-117">The label associated with Category 3</span></span>|
|<span data-ttu-id="950f4-118">category4</span><span class="sxs-lookup"><span data-stu-id="950f4-118">category4</span></span>|<span data-ttu-id="950f4-119">String</span><span class="sxs-lookup"><span data-stu-id="950f4-119">String</span></span>|<span data-ttu-id="950f4-120">Метка, сопоставленная с категорией 4.</span><span class="sxs-lookup"><span data-stu-id="950f4-120">The label associated with Category 4</span></span>|
|<span data-ttu-id="950f4-121">category5</span><span class="sxs-lookup"><span data-stu-id="950f4-121">category5</span></span>|<span data-ttu-id="950f4-122">String</span><span class="sxs-lookup"><span data-stu-id="950f4-122">String</span></span>|<span data-ttu-id="950f4-123">Метка, сопоставленная с категорией 5.</span><span class="sxs-lookup"><span data-stu-id="950f4-123">The label associated with Category 5</span></span>|
|<span data-ttu-id="950f4-124">category6</span><span class="sxs-lookup"><span data-stu-id="950f4-124">category6</span></span>|<span data-ttu-id="950f4-125">String</span><span class="sxs-lookup"><span data-stu-id="950f4-125">String</span></span>|<span data-ttu-id="950f4-126">Метка, сопоставленная с категорией 6.</span><span class="sxs-lookup"><span data-stu-id="950f4-126">The label associated with Category 6</span></span>|

## <span data-ttu-id="950f4-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="950f4-127">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="950f4-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="950f4-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->