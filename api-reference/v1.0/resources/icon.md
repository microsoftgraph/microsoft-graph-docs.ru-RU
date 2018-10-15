# <a name="icon-resource-type"></a><span data-ttu-id="3b07e-101">Тип ресурса Icon</span><span class="sxs-lookup"><span data-stu-id="3b07e-101">Icon resource type</span></span>

<span data-ttu-id="3b07e-102">Представляет значок ячейки.</span><span class="sxs-lookup"><span data-stu-id="3b07e-102">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="3b07e-103">Методы</span><span class="sxs-lookup"><span data-stu-id="3b07e-103">Methods</span></span>

| <span data-ttu-id="3b07e-104">Метод</span><span class="sxs-lookup"><span data-stu-id="3b07e-104">Method</span></span>           | <span data-ttu-id="3b07e-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b07e-105">Return Type</span></span>    |<span data-ttu-id="3b07e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="3b07e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b07e-107">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="3b07e-107">Get Icon</span></span>](../api/icon_get.md) | [<span data-ttu-id="3b07e-108">Значок</span><span class="sxs-lookup"><span data-stu-id="3b07e-108">Icon</span></span>](icon.md) |<span data-ttu-id="3b07e-109">Чтение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="3b07e-109">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="3b07e-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="3b07e-110">Update</span></span>](../api/icon_update.md) | [<span data-ttu-id="3b07e-111">Значок</span><span class="sxs-lookup"><span data-stu-id="3b07e-111">Icon</span></span>](icon.md)  |<span data-ttu-id="3b07e-112">Обновление объекта значка.</span><span class="sxs-lookup"><span data-stu-id="3b07e-112">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b07e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b07e-113">Properties</span></span>
| <span data-ttu-id="3b07e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b07e-114">Property</span></span>     | <span data-ttu-id="3b07e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3b07e-115">Type</span></span>   |<span data-ttu-id="3b07e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3b07e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b07e-117">index</span><span class="sxs-lookup"><span data-stu-id="3b07e-117">index</span></span>|<span data-ttu-id="3b07e-118">int</span><span class="sxs-lookup"><span data-stu-id="3b07e-118">int</span></span>|<span data-ttu-id="3b07e-119">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="3b07e-119">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="3b07e-120">set</span><span class="sxs-lookup"><span data-stu-id="3b07e-120">set</span></span>|<span data-ttu-id="3b07e-121">string</span><span class="sxs-lookup"><span data-stu-id="3b07e-121">string</span></span>|<span data-ttu-id="3b07e-122">Представляет множество, частью которого является этот значок.</span><span class="sxs-lookup"><span data-stu-id="3b07e-122">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="3b07e-123">Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="3b07e-123">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b07e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3b07e-124">Relationships</span></span>
<span data-ttu-id="3b07e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3b07e-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b07e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b07e-126">JSON representation</span></span>

<span data-ttu-id="3b07e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b07e-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->