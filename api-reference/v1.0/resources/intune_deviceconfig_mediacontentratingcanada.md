# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="1e763-101">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1e763-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="1e763-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e763-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e763-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1e763-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1e763-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e763-104">Properties</span></span>
|<span data-ttu-id="1e763-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e763-105">Property</span></span>|<span data-ttu-id="1e763-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1e763-106">Type</span></span>|<span data-ttu-id="1e763-107">Описание</span><span class="sxs-lookup"><span data-stu-id="1e763-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e763-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="1e763-108">movieRating</span></span>|[<span data-ttu-id="1e763-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="1e763-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="1e763-110">Рейтинг фильмов, выбранный для Канады.</span><span class="sxs-lookup"><span data-stu-id="1e763-110">Movies rating selected for Canada Possible values are: , , , , , , .</span></span> <span data-ttu-id="1e763-111">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="1e763-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`, , , , , or .</span></span>|
|<span data-ttu-id="1e763-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="1e763-112">tvRating</span></span>|[<span data-ttu-id="1e763-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1e763-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="1e763-114">Оценка телепрограмм, выбранных для Канады.</span><span class="sxs-lookup"><span data-stu-id="1e763-114">TV rating selected for Canada Possible values are: , , , , , , , .</span></span> <span data-ttu-id="1e763-115">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1e763-115">The possible values are `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e763-116">Связи</span><span class="sxs-lookup"><span data-stu-id="1e763-116">Relationships</span></span>
<span data-ttu-id="1e763-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1e763-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e763-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e763-118">JSON Representation</span></span>
<span data-ttu-id="1e763-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e763-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



