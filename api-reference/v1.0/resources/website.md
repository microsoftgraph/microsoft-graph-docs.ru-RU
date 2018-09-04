# <a name="website-resource-type"></a><span data-ttu-id="337c2-101">Тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="337c2-101">website resource type</span></span>

<span data-ttu-id="337c2-102">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="337c2-102">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="337c2-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="337c2-103">Properties</span></span>
| <span data-ttu-id="337c2-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="337c2-104">Property</span></span>     | <span data-ttu-id="337c2-105">Тип</span><span class="sxs-lookup"><span data-stu-id="337c2-105">Type</span></span>   |<span data-ttu-id="337c2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="337c2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="337c2-107">type</span><span class="sxs-lookup"><span data-stu-id="337c2-107">type</span></span>|<span data-ttu-id="337c2-108">websiteType</span><span class="sxs-lookup"><span data-stu-id="337c2-108">websiteType values</span></span>| <span data-ttu-id="337c2-109">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="337c2-109">The possible values are `other`, `home`, `work`, `blog`, `profile`, , , , , , , or .</span></span>|
|<span data-ttu-id="337c2-110">address</span><span class="sxs-lookup"><span data-stu-id="337c2-110">address</span></span>|<span data-ttu-id="337c2-111">string (строка)</span><span class="sxs-lookup"><span data-stu-id="337c2-111">string</span></span>|<span data-ttu-id="337c2-112">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="337c2-112">The URL of the website.</span></span>|
|<span data-ttu-id="337c2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="337c2-113">displayName</span></span>|<span data-ttu-id="337c2-114">string (строка)</span><span class="sxs-lookup"><span data-stu-id="337c2-114">string</span></span>|<span data-ttu-id="337c2-115">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="337c2-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="337c2-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="337c2-116">JSON representation</span></span>

<span data-ttu-id="337c2-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="337c2-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
