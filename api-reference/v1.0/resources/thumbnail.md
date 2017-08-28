# <a name="thumbnail-resource-type"></a><span data-ttu-id="807dc-101">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="807dc-101">Thumbnail resource type</span></span>

<span data-ttu-id="807dc-102">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="807dc-102">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="807dc-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="807dc-103">JSON representation</span></span>

<span data-ttu-id="807dc-104">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="807dc-104">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="807dc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="807dc-105">Properties</span></span>

| <span data-ttu-id="807dc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="807dc-106">Property</span></span>     | <span data-ttu-id="807dc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="807dc-107">Type</span></span>   | <span data-ttu-id="807dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="807dc-108">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="807dc-109">height</span><span class="sxs-lookup"><span data-stu-id="807dc-109">height</span></span>       | <span data-ttu-id="807dc-110">Int32</span><span class="sxs-lookup"><span data-stu-id="807dc-110">Int32</span></span>  | <span data-ttu-id="807dc-111">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="807dc-111">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="807dc-112">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="807dc-112">sourceItemId</span></span> | <span data-ttu-id="807dc-113">String</span><span class="sxs-lookup"><span data-stu-id="807dc-113">String</span></span> | <span data-ttu-id="807dc-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="807dc-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="807dc-116">url</span><span class="sxs-lookup"><span data-stu-id="807dc-116">url</span></span>          | <span data-ttu-id="807dc-117">String</span><span class="sxs-lookup"><span data-stu-id="807dc-117">String</span></span> | <span data-ttu-id="807dc-118">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="807dc-118">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="807dc-119">width</span><span class="sxs-lookup"><span data-stu-id="807dc-119">width</span></span>        | <span data-ttu-id="807dc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="807dc-120">Int32</span></span>  | <span data-ttu-id="807dc-121">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="807dc-121">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="807dc-122">Связи</span><span class="sxs-lookup"><span data-stu-id="807dc-122">Relationships</span></span>

| <span data-ttu-id="807dc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="807dc-123">Name</span></span>    | <span data-ttu-id="807dc-124">Тип</span><span class="sxs-lookup"><span data-stu-id="807dc-124">Type</span></span>   | <span data-ttu-id="807dc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="807dc-125">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="807dc-126">content</span><span class="sxs-lookup"><span data-stu-id="807dc-126">content</span></span> | <span data-ttu-id="807dc-127">Stream</span><span class="sxs-lookup"><span data-stu-id="807dc-127">Stream</span></span> | <span data-ttu-id="807dc-128">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="807dc-128">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
