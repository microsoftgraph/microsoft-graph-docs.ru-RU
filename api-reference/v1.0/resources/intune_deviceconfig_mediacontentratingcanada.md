# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="72a52-101">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="72a52-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="72a52-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="72a52-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72a52-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="72a52-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="72a52-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="72a52-104">Properties</span></span>
|<span data-ttu-id="72a52-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="72a52-105">Property</span></span>|<span data-ttu-id="72a52-106">Тип</span><span class="sxs-lookup"><span data-stu-id="72a52-106">Type</span></span>|<span data-ttu-id="72a52-107">Описание</span><span class="sxs-lookup"><span data-stu-id="72a52-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72a52-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="72a52-108">movieRating</span></span>|<span data-ttu-id="72a52-109">String</span><span class="sxs-lookup"><span data-stu-id="72a52-109">String</span></span>|<span data-ttu-id="72a52-110">Рейтинг фильма для Канады. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="72a52-110">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="72a52-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="72a52-111">tvRating</span></span>|<span data-ttu-id="72a52-112">String</span><span class="sxs-lookup"><span data-stu-id="72a52-112">String</span></span>|<span data-ttu-id="72a52-113">Телевизионный рейтинг для Канады. Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="72a52-113">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72a52-114">Связи</span><span class="sxs-lookup"><span data-stu-id="72a52-114">Relationships</span></span>
<span data-ttu-id="72a52-115">Нет</span><span class="sxs-lookup"><span data-stu-id="72a52-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72a52-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72a52-116">JSON Representation</span></span>
<span data-ttu-id="72a52-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72a52-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



