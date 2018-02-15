# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="23552-101">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="23552-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="23552-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23552-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23552-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23552-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="23552-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="23552-104">Properties</span></span>
|<span data-ttu-id="23552-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="23552-105">Property</span></span>|<span data-ttu-id="23552-106">Тип</span><span class="sxs-lookup"><span data-stu-id="23552-106">Type</span></span>|<span data-ttu-id="23552-107">Описание</span><span class="sxs-lookup"><span data-stu-id="23552-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23552-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="23552-108">movieRating</span></span>|<span data-ttu-id="23552-109">String</span><span class="sxs-lookup"><span data-stu-id="23552-109">String</span></span>|<span data-ttu-id="23552-110">Рейтинг фильма для Соединенного Королевства. Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="23552-110">Movies rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="23552-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="23552-111">tvRating</span></span>|<span data-ttu-id="23552-112">String</span><span class="sxs-lookup"><span data-stu-id="23552-112">String</span></span>|<span data-ttu-id="23552-113">Телевизионный рейтинг для Соединенного Королевства. Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="23552-113">TV rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23552-114">Связи</span><span class="sxs-lookup"><span data-stu-id="23552-114">Relationships</span></span>
<span data-ttu-id="23552-115">Нет</span><span class="sxs-lookup"><span data-stu-id="23552-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23552-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23552-116">JSON Representation</span></span>
<span data-ttu-id="23552-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23552-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



