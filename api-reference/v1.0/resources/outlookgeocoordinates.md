# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="5513f-101">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5513f-101">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="5513f-102">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="5513f-102">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5513f-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5513f-103">JSON representation</span></span>

<span data-ttu-id="5513f-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5513f-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="5513f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5513f-105">Properties</span></span>
| <span data-ttu-id="5513f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5513f-106">Property</span></span>     | <span data-ttu-id="5513f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5513f-107">Type</span></span>   |<span data-ttu-id="5513f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5513f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5513f-109">accuracy</span><span class="sxs-lookup"><span data-stu-id="5513f-109">accuracy</span></span>|<span data-ttu-id="5513f-110">double</span><span class="sxs-lookup"><span data-stu-id="5513f-110">double</span></span>|<span data-ttu-id="5513f-111">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="5513f-111">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="5513f-112">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="5513f-112">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="5513f-113">altitude</span><span class="sxs-lookup"><span data-stu-id="5513f-113">altitude</span></span>|<span data-ttu-id="5513f-114">double</span><span class="sxs-lookup"><span data-stu-id="5513f-114">double</span></span>|<span data-ttu-id="5513f-115">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="5513f-115">The altitude of the location.</span></span>|
|<span data-ttu-id="5513f-116">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="5513f-116">altitudeAccuracy</span></span>|<span data-ttu-id="5513f-117">double</span><span class="sxs-lookup"><span data-stu-id="5513f-117">double</span></span>|<span data-ttu-id="5513f-118">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="5513f-118">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="5513f-119">latitude</span><span class="sxs-lookup"><span data-stu-id="5513f-119">latitude</span></span>|<span data-ttu-id="5513f-120">double</span><span class="sxs-lookup"><span data-stu-id="5513f-120">double</span></span>|<span data-ttu-id="5513f-121">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="5513f-121">The latitude of the location.</span></span>|
|<span data-ttu-id="5513f-122">longitude</span><span class="sxs-lookup"><span data-stu-id="5513f-122">longitude</span></span>|<span data-ttu-id="5513f-123">double</span><span class="sxs-lookup"><span data-stu-id="5513f-123">double</span></span>|<span data-ttu-id="5513f-124">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="5513f-124">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->