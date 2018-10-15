# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="084fb-101">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="084fb-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="084fb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="084fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="084fb-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="084fb-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="084fb-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="084fb-104">Properties</span></span>
|<span data-ttu-id="084fb-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="084fb-105">Property</span></span>|<span data-ttu-id="084fb-106">Тип</span><span class="sxs-lookup"><span data-stu-id="084fb-106">Type</span></span>|<span data-ttu-id="084fb-107">Описание</span><span class="sxs-lookup"><span data-stu-id="084fb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="084fb-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="084fb-108">movieRating</span></span>|[<span data-ttu-id="084fb-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="084fb-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="084fb-p101">Рейтинг фильмов, отобранных для Германии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="084fb-p101">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="084fb-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="084fb-112">tvRating</span></span>|[<span data-ttu-id="084fb-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="084fb-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="084fb-p102">Рейтинг ТВ-программ, отобранных для Германии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="084fb-p102">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="084fb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="084fb-116">Relationships</span></span>
<span data-ttu-id="084fb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="084fb-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="084fb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="084fb-118">JSON Representation</span></span>
<span data-ttu-id="084fb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="084fb-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```








