# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="72814-101">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="72814-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="72814-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="72814-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72814-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="72814-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="72814-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="72814-104">Properties</span></span>
|<span data-ttu-id="72814-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="72814-105">Property</span></span>|<span data-ttu-id="72814-106">Тип</span><span class="sxs-lookup"><span data-stu-id="72814-106">Type</span></span>|<span data-ttu-id="72814-107">Описание</span><span class="sxs-lookup"><span data-stu-id="72814-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72814-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="72814-108">movieRating</span></span>|<span data-ttu-id="72814-109">String</span><span class="sxs-lookup"><span data-stu-id="72814-109">String</span></span>|<span data-ttu-id="72814-110">Рейтинг фильма для Японии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="72814-110">Movies rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="72814-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="72814-111">tvRating</span></span>|<span data-ttu-id="72814-112">String</span><span class="sxs-lookup"><span data-stu-id="72814-112">String</span></span>|<span data-ttu-id="72814-113">Телевизионный рейтинг для Японии. Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="72814-113">TV rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72814-114">Связи</span><span class="sxs-lookup"><span data-stu-id="72814-114">Relationships</span></span>
<span data-ttu-id="72814-115">Нет</span><span class="sxs-lookup"><span data-stu-id="72814-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72814-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72814-116">JSON Representation</span></span>
<span data-ttu-id="72814-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72814-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



