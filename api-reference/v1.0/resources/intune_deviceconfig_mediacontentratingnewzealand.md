# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="2a66a-101">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="2a66a-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="2a66a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a66a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a66a-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a66a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2a66a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a66a-104">Properties</span></span>
|<span data-ttu-id="2a66a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a66a-105">Property</span></span>|<span data-ttu-id="2a66a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2a66a-106">Type</span></span>|<span data-ttu-id="2a66a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2a66a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a66a-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2a66a-108">movieRating</span></span>|[<span data-ttu-id="2a66a-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="2a66a-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="2a66a-110">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="2a66a-110">Movies rating selected for New Zealand Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="2a66a-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="2a66a-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`, or .</span></span>|
|<span data-ttu-id="2a66a-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="2a66a-112">tvRating</span></span>|[<span data-ttu-id="2a66a-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2a66a-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="2a66a-114">Рейтинг телепередач, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="2a66a-114">TV rating selected for New Zealand Possible values are: , , , , .</span></span> <span data-ttu-id="2a66a-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2a66a-115">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a66a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2a66a-116">Relationships</span></span>
<span data-ttu-id="2a66a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2a66a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a66a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a66a-118">JSON Representation</span></span>
<span data-ttu-id="2a66a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a66a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



