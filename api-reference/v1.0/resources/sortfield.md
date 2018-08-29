# <a name="sortfield-resource-type"></a><span data-ttu-id="f1ea7-101">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="f1ea7-101">SortField resource type</span></span>

<span data-ttu-id="f1ea7-102">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-102">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="f1ea7-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1ea7-103">Properties</span></span>
| <span data-ttu-id="f1ea7-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1ea7-104">Property</span></span>     | <span data-ttu-id="f1ea7-105">Тип</span><span class="sxs-lookup"><span data-stu-id="f1ea7-105">Type</span></span>   |<span data-ttu-id="f1ea7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ea7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1ea7-107">ascending</span><span class="sxs-lookup"><span data-stu-id="f1ea7-107">ascending</span></span>|<span data-ttu-id="f1ea7-108">логический</span><span class="sxs-lookup"><span data-stu-id="f1ea7-108">boolean</span></span>|<span data-ttu-id="f1ea7-109">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-109">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="f1ea7-110">color</span><span class="sxs-lookup"><span data-stu-id="f1ea7-110">color</span></span>|<span data-ttu-id="f1ea7-111">строка</span><span class="sxs-lookup"><span data-stu-id="f1ea7-111">string</span></span>|<span data-ttu-id="f1ea7-112">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-112">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="f1ea7-113">dataOption</span><span class="sxs-lookup"><span data-stu-id="f1ea7-113">dataOption</span></span>|<span data-ttu-id="f1ea7-114">строка</span><span class="sxs-lookup"><span data-stu-id="f1ea7-114">string</span></span>|<span data-ttu-id="f1ea7-115">Представляет дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-115">Represents additional sorting options for this field. Possible values are: , .</span></span> <span data-ttu-id="f1ea7-116">Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-116">The possible values are:</span></span>|
|<span data-ttu-id="f1ea7-117">key</span><span class="sxs-lookup"><span data-stu-id="f1ea7-117">key</span></span>|<span data-ttu-id="f1ea7-118">int</span><span class="sxs-lookup"><span data-stu-id="f1ea7-118">int</span></span>|<span data-ttu-id="f1ea7-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="f1ea7-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="f1ea7-121">sortOn</span><span class="sxs-lookup"><span data-stu-id="f1ea7-121">sortOn</span></span>|<span data-ttu-id="f1ea7-122">строка</span><span class="sxs-lookup"><span data-stu-id="f1ea7-122">string</span></span>|<span data-ttu-id="f1ea7-123">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-123">Represents the type of sorting of this condition. Possible values are: , , , .</span></span> <span data-ttu-id="f1ea7-124">Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-124">The possible values are `Value`, `CellColor`, `FontColor`, `Icon`, , , , , , , , or .</span></span>|
|<span data-ttu-id="f1ea7-125">icon</span><span class="sxs-lookup"><span data-stu-id="f1ea7-125">icon</span></span>|[<span data-ttu-id="f1ea7-126">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="f1ea7-126">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="f1ea7-127">Представляет целевой значок условия при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-127">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1ea7-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1ea7-128">JSON representation</span></span>

<span data-ttu-id="f1ea7-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1ea7-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->