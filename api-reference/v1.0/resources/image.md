# <a name="image-resource-type"></a><span data-ttu-id="1dde9-101">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="1dde9-101">Image resource type</span></span>

<span data-ttu-id="1dde9-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="1dde9-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="1dde9-104">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="1dde9-104">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dde9-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dde9-105">JSON representation</span></span>

<span data-ttu-id="1dde9-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dde9-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a><span data-ttu-id="1dde9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dde9-107">Properties</span></span>

| <span data-ttu-id="1dde9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dde9-108">Property</span></span>   | <span data-ttu-id="1dde9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1dde9-109">Type</span></span>  | <span data-ttu-id="1dde9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1dde9-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="1dde9-111">**height**</span><span class="sxs-lookup"><span data-stu-id="1dde9-111">**height**</span></span> | <span data-ttu-id="1dde9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1dde9-112">Int32</span></span> | <span data-ttu-id="1dde9-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1dde9-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="1dde9-116">**width**</span><span class="sxs-lookup"><span data-stu-id="1dde9-116">**width**</span></span>  | <span data-ttu-id="1dde9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="1dde9-117">Int32</span></span> | <span data-ttu-id="1dde9-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1dde9-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="1dde9-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="1dde9-121">Remarks</span></span>

<span data-ttu-id="1dde9-p104">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла. В OneDrive для бизнеса этот ресурс не возвращает свойств.</span><span class="sxs-lookup"><span data-stu-id="1dde9-p104">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="1dde9-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1dde9-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
