# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="ed791-101">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ed791-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="ed791-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed791-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed791-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ed791-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ed791-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed791-104">Properties</span></span>
|<span data-ttu-id="ed791-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed791-105">Property</span></span>|<span data-ttu-id="ed791-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ed791-106">Type</span></span>|<span data-ttu-id="ed791-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ed791-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed791-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ed791-108">movieRating</span></span>|[<span data-ttu-id="ed791-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="ed791-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="ed791-110">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="ed791-110">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="ed791-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ed791-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="ed791-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="ed791-112">tvRating</span></span>|[<span data-ttu-id="ed791-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ed791-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="ed791-114">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="ed791-114">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="ed791-115">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="ed791-115">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed791-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ed791-116">Relationships</span></span>
<span data-ttu-id="ed791-117">None</span><span class="sxs-lookup"><span data-stu-id="ed791-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed791-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed791-118">JSON Representation</span></span>
<span data-ttu-id="ed791-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed791-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



