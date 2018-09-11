# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="7d07a-101">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="7d07a-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="7d07a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d07a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d07a-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7d07a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7d07a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d07a-104">Properties</span></span>
|<span data-ttu-id="7d07a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d07a-105">Property</span></span>|<span data-ttu-id="7d07a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7d07a-106">Type</span></span>|<span data-ttu-id="7d07a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7d07a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d07a-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="7d07a-108">movieRating</span></span>|[<span data-ttu-id="7d07a-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="7d07a-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="7d07a-p101">Телевизионный рейтинг для Ирландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7d07a-p101">Movies rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7d07a-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="7d07a-112">tvRating</span></span>|[<span data-ttu-id="7d07a-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7d07a-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="7d07a-p102">Телевизионный рейтинг для Ирландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="7d07a-p102">TV rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d07a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7d07a-116">Relationships</span></span>
<span data-ttu-id="7d07a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7d07a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d07a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d07a-118">JSON Representation</span></span>
<span data-ttu-id="7d07a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d07a-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```








