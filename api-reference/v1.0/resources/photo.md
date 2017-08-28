# <a name="photo-resource-type"></a><span data-ttu-id="0d4e7-101">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="0d4e7-101">Photo resource type</span></span>

<span data-ttu-id="0d4e7-102">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0d4e7-102">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d4e7-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d4e7-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="0d4e7-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d4e7-104">Properties</span></span>
| <span data-ttu-id="0d4e7-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4e7-105">Property</span></span>                | <span data-ttu-id="0d4e7-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4e7-106">Type</span></span>                      | <span data-ttu-id="0d4e7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4e7-107">Description</span></span>                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| <span data-ttu-id="0d4e7-108">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-108">**takenDateTime**</span></span>       | <span data-ttu-id="0d4e7-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d4e7-109">DateTimeOffset</span></span>            | <span data-ttu-id="0d4e7-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p101">Represents the date and time the photo was taken. Read-only.</span></span>               |
| <span data-ttu-id="0d4e7-112">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-112">**cameraMake**</span></span>          | <span data-ttu-id="0d4e7-113">String</span><span class="sxs-lookup"><span data-stu-id="0d4e7-113">String</span></span>                    | <span data-ttu-id="0d4e7-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p102">Camera manufacturer. Read-only.</span></span>                                            |
| <span data-ttu-id="0d4e7-116">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-116">**cameraModel**</span></span>         | <span data-ttu-id="0d4e7-117">String</span><span class="sxs-lookup"><span data-stu-id="0d4e7-117">String</span></span>                    | <span data-ttu-id="0d4e7-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p103">Camera model. Read-only.</span></span>                                                   |
| <span data-ttu-id="0d4e7-120">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-120">**fNumber**</span></span>             | <span data-ttu-id="0d4e7-121">Double</span><span class="sxs-lookup"><span data-stu-id="0d4e7-121">Double</span></span>                    | <span data-ttu-id="0d4e7-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p104">The F-stop value from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="0d4e7-124">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-124">**exposureDenominator**</span></span> | <span data-ttu-id="0d4e7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0d4e7-125">Int32</span></span>                     | <span data-ttu-id="0d4e7-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
| <span data-ttu-id="0d4e7-128">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-128">**exposureNumerator**</span></span>   | <span data-ttu-id="0d4e7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0d4e7-129">Int32</span></span>                     | <span data-ttu-id="0d4e7-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
| <span data-ttu-id="0d4e7-132">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-132">**focalLength**</span></span>         | <span data-ttu-id="0d4e7-133">Double</span><span class="sxs-lookup"><span data-stu-id="0d4e7-133">Double</span></span>                    | <span data-ttu-id="0d4e7-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p107">The focal length from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="0d4e7-136">**iso**</span><span class="sxs-lookup"><span data-stu-id="0d4e7-136">**iso**</span></span>                 | <span data-ttu-id="0d4e7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0d4e7-137">Int32</span></span>                     | <span data-ttu-id="0d4e7-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-p108">The ISO value from the camera. Read-only.</span></span>                                  |

## <a name="remarks"></a><span data-ttu-id="0d4e7-140">Заметки</span><span class="sxs-lookup"><span data-stu-id="0d4e7-140">Remarks</span></span>
<span data-ttu-id="0d4e7-141">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="0d4e7-141">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="0d4e7-142">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0d4e7-142">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
