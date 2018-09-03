# <a name="rangefill-resource-type"></a><span data-ttu-id="c09ae-101">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="c09ae-101">RangeFill resource type</span></span>

<span data-ttu-id="c09ae-102">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="c09ae-102">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="c09ae-103">Методы</span><span class="sxs-lookup"><span data-stu-id="c09ae-103">Methods</span></span>

| <span data-ttu-id="c09ae-104">Метод</span><span class="sxs-lookup"><span data-stu-id="c09ae-104">Method</span></span>           | <span data-ttu-id="c09ae-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c09ae-105">Return Type</span></span>    |<span data-ttu-id="c09ae-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c09ae-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c09ae-107">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="c09ae-107">Get RangeFill</span></span>](../api/rangefill_get.md) | [<span data-ttu-id="c09ae-108">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="c09ae-108">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="c09ae-109">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="c09ae-109">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="c09ae-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="c09ae-110">Update</span></span>](../api/rangefill_update.md) | [<span data-ttu-id="c09ae-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="c09ae-111">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="c09ae-112">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="c09ae-112">Update RangeFill object.</span></span> |
|[<span data-ttu-id="c09ae-113">Очистить</span><span class="sxs-lookup"><span data-stu-id="c09ae-113">Clear</span></span>](../api/rangefill_clear.md)|<span data-ttu-id="c09ae-114">Нет</span><span class="sxs-lookup"><span data-stu-id="c09ae-114">None</span></span>|<span data-ttu-id="c09ae-115">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="c09ae-115">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="c09ae-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c09ae-116">Properties</span></span>
| <span data-ttu-id="c09ae-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c09ae-117">Property</span></span>     | <span data-ttu-id="c09ae-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c09ae-118">Type</span></span>   |<span data-ttu-id="c09ae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c09ae-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c09ae-120">color</span><span class="sxs-lookup"><span data-stu-id="c09ae-120">color</span></span>|<span data-ttu-id="c09ae-121">строка</span><span class="sxs-lookup"><span data-stu-id="c09ae-121">string</span></span>|<span data-ttu-id="c09ae-122">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="c09ae-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="c09ae-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c09ae-123">Relationships</span></span>
<span data-ttu-id="c09ae-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c09ae-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c09ae-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c09ae-125">JSON representation</span></span>

<span data-ttu-id="c09ae-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c09ae-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->