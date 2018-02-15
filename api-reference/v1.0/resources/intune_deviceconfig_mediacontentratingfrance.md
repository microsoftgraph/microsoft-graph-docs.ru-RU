# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="c81a5-101">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c81a5-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="c81a5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c81a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c81a5-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c81a5-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c81a5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c81a5-104">Properties</span></span>
|<span data-ttu-id="c81a5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c81a5-105">Property</span></span>|<span data-ttu-id="c81a5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c81a5-106">Type</span></span>|<span data-ttu-id="c81a5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c81a5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c81a5-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c81a5-108">movieRating</span></span>|<span data-ttu-id="c81a5-109">String</span><span class="sxs-lookup"><span data-stu-id="c81a5-109">String</span></span>|<span data-ttu-id="c81a5-110">Рейтинг фильма для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c81a5-110">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c81a5-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="c81a5-111">tvRating</span></span>|<span data-ttu-id="c81a5-112">String</span><span class="sxs-lookup"><span data-stu-id="c81a5-112">String</span></span>|<span data-ttu-id="c81a5-113">Телевизионный рейтинг для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c81a5-113">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c81a5-114">Связи</span><span class="sxs-lookup"><span data-stu-id="c81a5-114">Relationships</span></span>
<span data-ttu-id="c81a5-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c81a5-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c81a5-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c81a5-116">JSON Representation</span></span>
<span data-ttu-id="c81a5-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c81a5-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



