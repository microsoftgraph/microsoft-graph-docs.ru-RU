# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="412a6-101">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="412a6-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="412a6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="412a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="412a6-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="412a6-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="412a6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="412a6-104">Properties</span></span>
|<span data-ttu-id="412a6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="412a6-105">Property</span></span>|<span data-ttu-id="412a6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="412a6-106">Type</span></span>|<span data-ttu-id="412a6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="412a6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412a6-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="412a6-108">movieRating</span></span>|[<span data-ttu-id="412a6-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="412a6-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="412a6-p101">Рейтинг выбранных фильмов для новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="412a6-p101">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="412a6-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="412a6-112">tvRating</span></span>|[<span data-ttu-id="412a6-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="412a6-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="412a6-p102">Рейтинг телевизионных передач для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="412a6-p102">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="412a6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="412a6-116">Relationships</span></span>
<span data-ttu-id="412a6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="412a6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="412a6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="412a6-118">JSON Representation</span></span>
<span data-ttu-id="412a6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="412a6-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








