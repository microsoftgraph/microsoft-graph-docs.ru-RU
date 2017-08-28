# <a name="thumbnailset-resource-type"></a><span data-ttu-id="f18ab-101">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="f18ab-101">ThumbnailSet resource type</span></span>

<span data-ttu-id="f18ab-p101">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="f18ab-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f18ab-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f18ab-104">JSON representation</span></span>

<span data-ttu-id="f18ab-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f18ab-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": {"@odata.type": "microsoft.graph.thumbnail"},
  "medium": {"@odata.type": "microsoft.graph.thumbnail"},
  "small": {"@odata.type": "microsoft.graph.thumbnail"},
  "source": {"@odata.type": "microsoft.graph.thumbnail"}
}
```

## <a name="properties"></a><span data-ttu-id="f18ab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f18ab-106">Properties</span></span>

| <span data-ttu-id="f18ab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f18ab-107">Property</span></span> | <span data-ttu-id="f18ab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f18ab-108">Type</span></span>                      | <span data-ttu-id="f18ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f18ab-109">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="f18ab-110">id</span><span class="sxs-lookup"><span data-stu-id="f18ab-110">id</span></span>       | <span data-ttu-id="f18ab-111">String</span><span class="sxs-lookup"><span data-stu-id="f18ab-111">String</span></span>                    | <span data-ttu-id="f18ab-p102">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f18ab-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="f18ab-114">large</span><span class="sxs-lookup"><span data-stu-id="f18ab-114">large</span></span>    | [<span data-ttu-id="f18ab-115">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="f18ab-115">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ab-116">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="f18ab-116">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="f18ab-117">medium</span><span class="sxs-lookup"><span data-stu-id="f18ab-117">medium</span></span>   | [<span data-ttu-id="f18ab-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="f18ab-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ab-119">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="f18ab-119">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="f18ab-120">small</span><span class="sxs-lookup"><span data-stu-id="f18ab-120">small</span></span>    | [<span data-ttu-id="f18ab-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="f18ab-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ab-122">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="f18ab-122">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="f18ab-123">source</span><span class="sxs-lookup"><span data-stu-id="f18ab-123">source</span></span>   | [<span data-ttu-id="f18ab-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="f18ab-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ab-125">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="f18ab-125">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
