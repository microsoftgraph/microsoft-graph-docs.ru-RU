# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="09bc8-101">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="09bc8-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="09bc8-102">**Примечание.** для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09bc8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09bc8-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="09bc8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="09bc8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="09bc8-104">Properties</span></span>
|<span data-ttu-id="09bc8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="09bc8-105">Property</span></span>|<span data-ttu-id="09bc8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="09bc8-106">Type</span></span>|<span data-ttu-id="09bc8-107">Описание</span><span class="sxs-lookup"><span data-stu-id="09bc8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09bc8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="09bc8-108">movieRating</span></span>|[<span data-ttu-id="09bc8-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="09bc8-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="09bc8-p101">Рейтинг фильма для Австралии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="09bc8-p101">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="09bc8-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="09bc8-112">tvRating</span></span>|[<span data-ttu-id="09bc8-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="09bc8-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="09bc8-p102">Рейтинг фильма для Австралии. Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="09bc8-p102">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09bc8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="09bc8-116">Relationships</span></span>
<span data-ttu-id="09bc8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="09bc8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09bc8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09bc8-118">JSON Representation</span></span>
<span data-ttu-id="09bc8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09bc8-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```








