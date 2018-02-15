# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="945f8-101">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="945f8-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="945f8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="945f8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="945f8-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945f8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="945f8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="945f8-104">Properties</span></span>
|<span data-ttu-id="945f8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="945f8-105">Property</span></span>|<span data-ttu-id="945f8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="945f8-106">Type</span></span>|<span data-ttu-id="945f8-107">Описание</span><span class="sxs-lookup"><span data-stu-id="945f8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="945f8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="945f8-108">movieRating</span></span>|<span data-ttu-id="945f8-109">String</span><span class="sxs-lookup"><span data-stu-id="945f8-109">String</span></span>|<span data-ttu-id="945f8-110">Рейтинг фильма для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="945f8-110">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="945f8-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="945f8-111">tvRating</span></span>|<span data-ttu-id="945f8-112">String</span><span class="sxs-lookup"><span data-stu-id="945f8-112">String</span></span>|<span data-ttu-id="945f8-113">Телевизионный рейтинг для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="945f8-113">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="945f8-114">Связи</span><span class="sxs-lookup"><span data-stu-id="945f8-114">Relationships</span></span>
<span data-ttu-id="945f8-115">Нет</span><span class="sxs-lookup"><span data-stu-id="945f8-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="945f8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="945f8-116">JSON Representation</span></span>
<span data-ttu-id="945f8-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="945f8-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



