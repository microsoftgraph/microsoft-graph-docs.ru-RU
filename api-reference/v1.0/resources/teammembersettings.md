# <a name="teammembersettings-resource-type"></a><span data-ttu-id="0c2d3-101">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="0c2d3-101">teamMemberSettings resource type</span></span>



<span data-ttu-id="0c2d3-102">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="0c2d3-102">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0c2d3-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c2d3-103">Properties</span></span>
| <span data-ttu-id="0c2d3-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c2d3-104">Property</span></span>     | <span data-ttu-id="0c2d3-105">Тип</span><span class="sxs-lookup"><span data-stu-id="0c2d3-105">Type</span></span>   |<span data-ttu-id="0c2d3-106">Описание</span><span class="sxs-lookup"><span data-stu-id="0c2d3-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c2d3-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="0c2d3-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="0c2d3-108">Логический</span><span class="sxs-lookup"><span data-stu-id="0c2d3-108">Boolean</span></span>|<span data-ttu-id="0c2d3-109">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-109">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="0c2d3-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="0c2d3-110">allowDeleteChannels</span></span>|<span data-ttu-id="0c2d3-111">Логический</span><span class="sxs-lookup"><span data-stu-id="0c2d3-111">Boolean</span></span>|<span data-ttu-id="0c2d3-112">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-112">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="0c2d3-113">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="0c2d3-113">allowAddRemoveApps</span></span>|<span data-ttu-id="0c2d3-114">Логический</span><span class="sxs-lookup"><span data-stu-id="0c2d3-114">Boolean</span></span>|<span data-ttu-id="0c2d3-115">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-115">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="0c2d3-116">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="0c2d3-116">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="0c2d3-117">Логический</span><span class="sxs-lookup"><span data-stu-id="0c2d3-117">Boolean</span></span>|<span data-ttu-id="0c2d3-118">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-118">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="0c2d3-119">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="0c2d3-119">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="0c2d3-120">Логический</span><span class="sxs-lookup"><span data-stu-id="0c2d3-120">Boolean</span></span>|<span data-ttu-id="0c2d3-121">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-121">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c2d3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c2d3-122">JSON representation</span></span>

<span data-ttu-id="0c2d3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c2d3-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
