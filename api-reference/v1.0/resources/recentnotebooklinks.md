# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="7b43d-101">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="7b43d-101">recentNotebookLinks resource type</span></span>

<span data-ttu-id="7b43d-102">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="7b43d-102">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="7b43d-103">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="7b43d-103">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7b43d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b43d-104">Properties</span></span>
| <span data-ttu-id="7b43d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b43d-105">Property</span></span>     | <span data-ttu-id="7b43d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7b43d-106">Type</span></span>   |<span data-ttu-id="7b43d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7b43d-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b43d-108">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="7b43d-108">oneNoteClientUrl</span></span>|[<span data-ttu-id="7b43d-109">externalLink</span><span class="sxs-lookup"><span data-stu-id="7b43d-109">externalLink</span></span>](externallink.md)|<span data-ttu-id="7b43d-110">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="7b43d-110">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="7b43d-111">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="7b43d-111">oneNoteWebUrl</span></span>|[<span data-ttu-id="7b43d-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="7b43d-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="7b43d-113">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="7b43d-113">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b43d-114">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b43d-114">JSON representation</span></span>

<span data-ttu-id="7b43d-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b43d-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
