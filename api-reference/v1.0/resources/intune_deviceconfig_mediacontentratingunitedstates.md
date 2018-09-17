# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="5998e-101">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="5998e-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="5998e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5998e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5998e-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5998e-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5998e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="5998e-104">Properties</span></span>
|<span data-ttu-id="5998e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="5998e-105">Property</span></span>|<span data-ttu-id="5998e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5998e-106">Type</span></span>|<span data-ttu-id="5998e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="5998e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5998e-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="5998e-108">movieRating</span></span>|[<span data-ttu-id="5998e-109">оценка типа фильма в США</span><span class="sxs-lookup"><span data-stu-id="5998e-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="5998e-p101">Рейтинг фильмов, выбранных для США. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5998e-p101">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="5998e-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="5998e-112">tvRating</span></span>|[<span data-ttu-id="5998e-113">оценка типа телевидения в США</span><span class="sxs-lookup"><span data-stu-id="5998e-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="5998e-p102">Рейтинг ТВ-программ, выбранных для США. Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5998e-p102">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5998e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5998e-116">Relationships</span></span>
<span data-ttu-id="5998e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5998e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5998e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5998e-118">JSON Representation</span></span>
<span data-ttu-id="5998e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5998e-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```








