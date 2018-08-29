# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="bb90a-101">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="bb90a-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="bb90a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb90a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb90a-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bb90a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bb90a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb90a-104">Properties</span></span>
|<span data-ttu-id="bb90a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb90a-105">Property</span></span>|<span data-ttu-id="bb90a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bb90a-106">Type</span></span>|<span data-ttu-id="bb90a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="bb90a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb90a-108">оценка фильма</span><span class="sxs-lookup"><span data-stu-id="bb90a-108">movieRating</span></span>|[<span data-ttu-id="bb90a-109">оценка Тип фильма во Франции</span><span class="sxs-lookup"><span data-stu-id="bb90a-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="bb90a-110">Оценка выбранных для Франции фильмов.</span><span class="sxs-lookup"><span data-stu-id="bb90a-110">Movies rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="bb90a-111">Допустимые значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`,`agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bb90a-111">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="bb90a-112">тв оценка</span><span class="sxs-lookup"><span data-stu-id="bb90a-112">tvRating</span></span>|[<span data-ttu-id="bb90a-113">оценка типа телевидения во Франции</span><span class="sxs-lookup"><span data-stu-id="bb90a-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="bb90a-114">ТВ-оценка, выбранная для Франции.</span><span class="sxs-lookup"><span data-stu-id="bb90a-114">TV rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="bb90a-115">Допустимые значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`,`agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bb90a-115">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb90a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="bb90a-116">Relationships</span></span>
<span data-ttu-id="bb90a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="bb90a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb90a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb90a-118">JSON Representation</span></span>
<span data-ttu-id="bb90a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb90a-119">Here is a JSON representation of the resource.</span></span>
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



