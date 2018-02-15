# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="7f001-101">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7f001-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="7f001-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f001-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f001-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7f001-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7f001-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f001-104">Properties</span></span>
|<span data-ttu-id="7f001-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f001-105">Property</span></span>|<span data-ttu-id="7f001-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7f001-106">Type</span></span>|<span data-ttu-id="7f001-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7f001-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f001-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="7f001-108">movieRating</span></span>|<span data-ttu-id="7f001-109">String</span><span class="sxs-lookup"><span data-stu-id="7f001-109">String</span></span>|<span data-ttu-id="7f001-110">Рейтинг фильма для Австралии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="7f001-110">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="7f001-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="7f001-111">tvRating</span></span>|<span data-ttu-id="7f001-112">String</span><span class="sxs-lookup"><span data-stu-id="7f001-112">String</span></span>|<span data-ttu-id="7f001-113">Телевизионный рейтинг для Австралии. Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="7f001-113">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f001-114">Связи</span><span class="sxs-lookup"><span data-stu-id="7f001-114">Relationships</span></span>
<span data-ttu-id="7f001-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7f001-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f001-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f001-116">JSON Representation</span></span>
<span data-ttu-id="7f001-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f001-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



