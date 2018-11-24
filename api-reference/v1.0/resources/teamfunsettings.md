# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="e8755-101">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e8755-101">teamFunSettings resource type</span></span>



<span data-ttu-id="e8755-102">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="e8755-102">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e8755-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8755-103">Properties</span></span>
| <span data-ttu-id="e8755-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8755-104">Property</span></span>     | <span data-ttu-id="e8755-105">Тип</span><span class="sxs-lookup"><span data-stu-id="e8755-105">Type</span></span>   |<span data-ttu-id="e8755-106">Описание</span><span class="sxs-lookup"><span data-stu-id="e8755-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8755-107">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="e8755-107">allowGiphy</span></span>|<span data-ttu-id="e8755-108">Логический</span><span class="sxs-lookup"><span data-stu-id="e8755-108">Boolean</span></span>|<span data-ttu-id="e8755-109">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="e8755-109">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="e8755-110">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="e8755-110">giphyContentRating</span></span>|<span data-ttu-id="e8755-111">String (enum)</span><span class="sxs-lookup"><span data-stu-id="e8755-111">String (enum)</span></span>|<span data-ttu-id="e8755-112">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="e8755-112">Giphy content rating.</span></span> <span data-ttu-id="e8755-113">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="e8755-113">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="e8755-114">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="e8755-114">allowStickersAndMemes</span></span>|<span data-ttu-id="e8755-115">Логический</span><span class="sxs-lookup"><span data-stu-id="e8755-115">Boolean</span></span>|<span data-ttu-id="e8755-116">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="e8755-116">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="e8755-117">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="e8755-117">allowCustomMemes</span></span>|<span data-ttu-id="e8755-118">Логический</span><span class="sxs-lookup"><span data-stu-id="e8755-118">Boolean</span></span>|<span data-ttu-id="e8755-119">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="e8755-119">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8755-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8755-120">JSON representation</span></span>

<span data-ttu-id="e8755-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8755-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
