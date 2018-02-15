# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="4f4de-101">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="4f4de-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="4f4de-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f4de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f4de-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4f4de-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4f4de-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f4de-104">Properties</span></span>
|<span data-ttu-id="4f4de-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f4de-105">Property</span></span>|<span data-ttu-id="4f4de-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4f4de-106">Type</span></span>|<span data-ttu-id="4f4de-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4f4de-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f4de-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="4f4de-108">movieRating</span></span>|<span data-ttu-id="4f4de-109">String</span><span class="sxs-lookup"><span data-stu-id="4f4de-109">String</span></span>|<span data-ttu-id="4f4de-110">Рейтинг фильма для Германии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4f4de-110">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="4f4de-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="4f4de-111">tvRating</span></span>|<span data-ttu-id="4f4de-112">String</span><span class="sxs-lookup"><span data-stu-id="4f4de-112">String</span></span>|<span data-ttu-id="4f4de-113">Телевизионный рейтинг для Германии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4f4de-113">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f4de-114">Связи</span><span class="sxs-lookup"><span data-stu-id="4f4de-114">Relationships</span></span>
<span data-ttu-id="4f4de-115">Нет</span><span class="sxs-lookup"><span data-stu-id="4f4de-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4f4de-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f4de-116">JSON Representation</span></span>
<span data-ttu-id="4f4de-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f4de-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



