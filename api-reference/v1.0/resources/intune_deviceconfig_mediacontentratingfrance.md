# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="23894-101">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="23894-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="23894-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23894-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23894-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23894-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="23894-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="23894-104">Properties</span></span>
|<span data-ttu-id="23894-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="23894-105">Property</span></span>|<span data-ttu-id="23894-106">Тип</span><span class="sxs-lookup"><span data-stu-id="23894-106">Type</span></span>|<span data-ttu-id="23894-107">Описание</span><span class="sxs-lookup"><span data-stu-id="23894-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23894-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="23894-108">movieRating</span></span>|[<span data-ttu-id="23894-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="23894-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="23894-110">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="23894-110">Movies rating selected for France.</span></span> <span data-ttu-id="23894-111">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="23894-111">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="23894-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="23894-112">tvRating</span></span>|[<span data-ttu-id="23894-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="23894-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="23894-114">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="23894-114">TV rating selected for France.</span></span> <span data-ttu-id="23894-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="23894-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23894-116">Связи</span><span class="sxs-lookup"><span data-stu-id="23894-116">Relationships</span></span>
<span data-ttu-id="23894-117">None</span><span class="sxs-lookup"><span data-stu-id="23894-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23894-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23894-118">JSON Representation</span></span>
<span data-ttu-id="23894-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23894-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



