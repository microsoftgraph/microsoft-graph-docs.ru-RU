# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="50905-101">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="50905-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="50905-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50905-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50905-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50905-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="50905-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="50905-104">Properties</span></span>
|<span data-ttu-id="50905-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="50905-105">Property</span></span>|<span data-ttu-id="50905-106">Тип</span><span class="sxs-lookup"><span data-stu-id="50905-106">Type</span></span>|<span data-ttu-id="50905-107">Описание</span><span class="sxs-lookup"><span data-stu-id="50905-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50905-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="50905-108">movieRating</span></span>|[<span data-ttu-id="50905-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="50905-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="50905-110">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="50905-110">Movies rating selected for Ireland.</span></span> <span data-ttu-id="50905-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="50905-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="50905-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="50905-112">tvRating</span></span>|[<span data-ttu-id="50905-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="50905-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="50905-114">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="50905-114">TV rating selected for Ireland.</span></span> <span data-ttu-id="50905-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="50905-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50905-116">Связи</span><span class="sxs-lookup"><span data-stu-id="50905-116">Relationships</span></span>
<span data-ttu-id="50905-117">None</span><span class="sxs-lookup"><span data-stu-id="50905-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="50905-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50905-118">JSON Representation</span></span>
<span data-ttu-id="50905-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50905-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



