# <a name="chartgridlines-resource-type"></a><span data-ttu-id="66ec2-101">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="66ec2-101">ChartGridlines resource type</span></span>

<span data-ttu-id="66ec2-102">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="66ec2-102">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="66ec2-103">Методы</span><span class="sxs-lookup"><span data-stu-id="66ec2-103">Methods</span></span>

| <span data-ttu-id="66ec2-104">Метод</span><span class="sxs-lookup"><span data-stu-id="66ec2-104">Method</span></span>           | <span data-ttu-id="66ec2-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66ec2-105">Return Type</span></span>    |<span data-ttu-id="66ec2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="66ec2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66ec2-107">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="66ec2-107">Get ChartGridlines</span></span>](../api/chartgridlines_get.md) | [<span data-ttu-id="66ec2-108">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="66ec2-108">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="66ec2-109">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="66ec2-109">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="66ec2-110">Update</span><span class="sxs-lookup"><span data-stu-id="66ec2-110">Update</span></span>](../api/chartgridlines_update.md) | [<span data-ttu-id="66ec2-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="66ec2-111">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="66ec2-112">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="66ec2-112">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66ec2-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="66ec2-113">Properties</span></span>
| <span data-ttu-id="66ec2-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="66ec2-114">Property</span></span>     | <span data-ttu-id="66ec2-115">Тип</span><span class="sxs-lookup"><span data-stu-id="66ec2-115">Type</span></span>   |<span data-ttu-id="66ec2-116">Описание</span><span class="sxs-lookup"><span data-stu-id="66ec2-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66ec2-117">видимый</span><span class="sxs-lookup"><span data-stu-id="66ec2-117">visible</span></span>|<span data-ttu-id="66ec2-118">boolean</span><span class="sxs-lookup"><span data-stu-id="66ec2-118">boolean</span></span>|<span data-ttu-id="66ec2-119">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="66ec2-119">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66ec2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="66ec2-120">Relationships</span></span>
| <span data-ttu-id="66ec2-121">Связь</span><span class="sxs-lookup"><span data-stu-id="66ec2-121">Relationship</span></span> | <span data-ttu-id="66ec2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="66ec2-122">Type</span></span>   |<span data-ttu-id="66ec2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="66ec2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66ec2-124">формат</span><span class="sxs-lookup"><span data-stu-id="66ec2-124">format</span></span>|[<span data-ttu-id="66ec2-125">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="66ec2-125">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="66ec2-p101">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66ec2-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66ec2-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66ec2-128">JSON representation</span></span>

<span data-ttu-id="66ec2-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66ec2-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->