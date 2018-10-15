# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="c0c3c-101">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="c0c3c-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="c0c3c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0c3c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0c3c-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0c3c-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c0c3c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0c3c-104">Properties</span></span>
|<span data-ttu-id="c0c3c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0c3c-105">Property</span></span>|<span data-ttu-id="c0c3c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c0c3c-106">Type</span></span>|<span data-ttu-id="c0c3c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c3c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c3c-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c0c3c-108">movieRating</span></span>|[<span data-ttu-id="c0c3c-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c0c3c-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="c0c3c-p101">Рейтинг фильмов для Канады. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="c0c3c-p101">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="c0c3c-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c0c3c-112">tvRating</span></span>|[<span data-ttu-id="c0c3c-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c0c3c-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="c0c3c-p102">Рейтинг ТВ для Канады. Возможные значения:`allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c0c3c-p102">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c3c-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c0c3c-116">Relationships</span></span>
<span data-ttu-id="c0c3c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c0c3c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0c3c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0c3c-118">JSON Representation</span></span>
<span data-ttu-id="c0c3c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0c3c-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```








