# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="03244-101">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="03244-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="03244-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03244-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03244-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="03244-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="03244-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="03244-104">Properties</span></span>
|<span data-ttu-id="03244-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="03244-105">Property</span></span>|<span data-ttu-id="03244-106">Тип</span><span class="sxs-lookup"><span data-stu-id="03244-106">Type</span></span>|<span data-ttu-id="03244-107">Описание</span><span class="sxs-lookup"><span data-stu-id="03244-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03244-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="03244-108">movieRating</span></span>|[<span data-ttu-id="03244-109">оценка Тип фильма во Франции</span><span class="sxs-lookup"><span data-stu-id="03244-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="03244-p101">Рейтинг фильма для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="03244-p101">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="03244-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="03244-112">tvRating</span></span>|[<span data-ttu-id="03244-113">оценка типа телевидения во Франции</span><span class="sxs-lookup"><span data-stu-id="03244-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="03244-p102">Рейтинг ТВ для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="03244-p102">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03244-116">Связи</span><span class="sxs-lookup"><span data-stu-id="03244-116">Relationships</span></span>
<span data-ttu-id="03244-117">Нет</span><span class="sxs-lookup"><span data-stu-id="03244-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03244-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03244-118">JSON Representation</span></span>
<span data-ttu-id="03244-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03244-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```








