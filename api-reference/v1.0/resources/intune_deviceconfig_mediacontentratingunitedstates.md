# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="36210-101">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="36210-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="36210-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36210-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36210-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36210-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="36210-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="36210-104">Properties</span></span>
|<span data-ttu-id="36210-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="36210-105">Property</span></span>|<span data-ttu-id="36210-106">Тип</span><span class="sxs-lookup"><span data-stu-id="36210-106">Type</span></span>|<span data-ttu-id="36210-107">Описание</span><span class="sxs-lookup"><span data-stu-id="36210-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36210-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="36210-108">movieRating</span></span>|<span data-ttu-id="36210-109">String</span><span class="sxs-lookup"><span data-stu-id="36210-109">String</span></span>|<span data-ttu-id="36210-110">Рейтинг фильма для США. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="36210-110">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="36210-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="36210-111">tvRating</span></span>|<span data-ttu-id="36210-112">String</span><span class="sxs-lookup"><span data-stu-id="36210-112">String</span></span>|<span data-ttu-id="36210-113">Телевизионный рейтинг для США. Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="36210-113">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36210-114">Связи</span><span class="sxs-lookup"><span data-stu-id="36210-114">Relationships</span></span>
<span data-ttu-id="36210-115">Нет</span><span class="sxs-lookup"><span data-stu-id="36210-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36210-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36210-116">JSON Representation</span></span>
<span data-ttu-id="36210-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36210-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



