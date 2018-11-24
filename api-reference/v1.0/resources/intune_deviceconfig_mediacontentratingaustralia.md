# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="19301-101">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="19301-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="19301-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19301-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19301-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19301-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="19301-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="19301-104">Properties</span></span>
|<span data-ttu-id="19301-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="19301-105">Property</span></span>|<span data-ttu-id="19301-106">Тип</span><span class="sxs-lookup"><span data-stu-id="19301-106">Type</span></span>|<span data-ttu-id="19301-107">Описание</span><span class="sxs-lookup"><span data-stu-id="19301-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19301-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="19301-108">movieRating</span></span>|[<span data-ttu-id="19301-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="19301-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="19301-110">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="19301-110">Movies rating selected for Australia.</span></span> <span data-ttu-id="19301-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="19301-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="19301-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="19301-112">tvRating</span></span>|[<span data-ttu-id="19301-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="19301-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="19301-114">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="19301-114">TV rating selected for Australia.</span></span> <span data-ttu-id="19301-115">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="19301-115">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19301-116">Связи</span><span class="sxs-lookup"><span data-stu-id="19301-116">Relationships</span></span>
<span data-ttu-id="19301-117">None</span><span class="sxs-lookup"><span data-stu-id="19301-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19301-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19301-118">JSON Representation</span></span>
<span data-ttu-id="19301-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19301-119">Here is a JSON representation of the resource.</span></span>
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



