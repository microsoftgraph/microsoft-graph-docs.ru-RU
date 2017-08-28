# <a name="geocoordinates-resource-type"></a><span data-ttu-id="c3be8-101">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c3be8-101">GeoCoordinates resource type</span></span>

<span data-ttu-id="c3be8-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="c3be8-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3be8-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3be8-104">JSON representation</span></span>

<span data-ttu-id="c3be8-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c3be8-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="c3be8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3be8-106">Properties</span></span>

| <span data-ttu-id="c3be8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3be8-107">Property</span></span>  | <span data-ttu-id="c3be8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c3be8-108">Type</span></span>   | <span data-ttu-id="c3be8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c3be8-109">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c3be8-110">altitude</span><span class="sxs-lookup"><span data-stu-id="c3be8-110">altitude</span></span>  | <span data-ttu-id="c3be8-111">Double</span><span class="sxs-lookup"><span data-stu-id="c3be8-111">Double</span></span> | <span data-ttu-id="c3be8-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3be8-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span> |
| <span data-ttu-id="c3be8-115">latitude</span><span class="sxs-lookup"><span data-stu-id="c3be8-115">latitude</span></span>  | <span data-ttu-id="c3be8-116">Double</span><span class="sxs-lookup"><span data-stu-id="c3be8-116">Double</span></span> | <span data-ttu-id="c3be8-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3be8-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>   |
| <span data-ttu-id="c3be8-120">longitude</span><span class="sxs-lookup"><span data-stu-id="c3be8-120">longitude</span></span> | <span data-ttu-id="c3be8-121">Double</span><span class="sxs-lookup"><span data-stu-id="c3be8-121">Double</span></span> | <span data-ttu-id="c3be8-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3be8-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="c3be8-125">Заметки</span><span class="sxs-lookup"><span data-stu-id="c3be8-125">Remarks</span></span>

<span data-ttu-id="c3be8-126">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c3be8-126">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
