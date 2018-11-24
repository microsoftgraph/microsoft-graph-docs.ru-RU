# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="46095-101">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="46095-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="46095-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46095-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46095-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="46095-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="46095-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="46095-104">Properties</span></span>
|<span data-ttu-id="46095-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="46095-105">Property</span></span>|<span data-ttu-id="46095-106">Тип</span><span class="sxs-lookup"><span data-stu-id="46095-106">Type</span></span>|<span data-ttu-id="46095-107">Описание</span><span class="sxs-lookup"><span data-stu-id="46095-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46095-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="46095-108">movieRating</span></span>|[<span data-ttu-id="46095-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="46095-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="46095-110">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="46095-110">Movies rating selected for Japan.</span></span> <span data-ttu-id="46095-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="46095-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="46095-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="46095-112">tvRating</span></span>|[<span data-ttu-id="46095-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="46095-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="46095-114">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="46095-114">TV rating selected for Japan.</span></span> <span data-ttu-id="46095-115">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="46095-115">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46095-116">Связи</span><span class="sxs-lookup"><span data-stu-id="46095-116">Relationships</span></span>
<span data-ttu-id="46095-117">None</span><span class="sxs-lookup"><span data-stu-id="46095-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46095-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46095-118">JSON Representation</span></span>
<span data-ttu-id="46095-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46095-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



