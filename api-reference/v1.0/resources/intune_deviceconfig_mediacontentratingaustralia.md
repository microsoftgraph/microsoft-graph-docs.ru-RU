# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="58e7f-101">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="58e7f-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="58e7f-102">**Примечание.** для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58e7f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58e7f-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="58e7f-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="58e7f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="58e7f-104">Properties</span></span>
|<span data-ttu-id="58e7f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="58e7f-105">Property</span></span>|<span data-ttu-id="58e7f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="58e7f-106">Type</span></span>|<span data-ttu-id="58e7f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="58e7f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58e7f-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="58e7f-108">movieRating</span></span>|[<span data-ttu-id="58e7f-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="58e7f-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="58e7f-110">Рейтинг фильмов для Австралии.</span><span class="sxs-lookup"><span data-stu-id="58e7f-110">Movies rating selected for Australia Possible values are: , , , , , , .</span></span> <span data-ttu-id="58e7f-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="58e7f-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`, , , , , or .</span></span>|
|<span data-ttu-id="58e7f-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="58e7f-112">tvRating</span></span>|[<span data-ttu-id="58e7f-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="58e7f-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="58e7f-114">Рейтинг телепередач для Австралии.</span><span class="sxs-lookup"><span data-stu-id="58e7f-114">TV rating selected for Australia Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="58e7f-115">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="58e7f-115">The possible values are `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`, , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="58e7f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="58e7f-116">Relationships</span></span>
<span data-ttu-id="58e7f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="58e7f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58e7f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58e7f-118">JSON Representation</span></span>
<span data-ttu-id="58e7f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58e7f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



