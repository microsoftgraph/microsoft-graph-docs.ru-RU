# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="b7c68-101">Тип ресурса teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="b7c68-101">teamMessagingSettings resource type</span></span>



<span data-ttu-id="b7c68-102">Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="b7c68-102">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b7c68-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7c68-103">Properties</span></span>
| <span data-ttu-id="b7c68-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7c68-104">Property</span></span>     | <span data-ttu-id="b7c68-105">Тип</span><span class="sxs-lookup"><span data-stu-id="b7c68-105">Type</span></span>   |<span data-ttu-id="b7c68-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c68-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c68-107">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="b7c68-107">allowUserEditMessages</span></span>|<span data-ttu-id="b7c68-108">Логический</span><span class="sxs-lookup"><span data-stu-id="b7c68-108">Boolean</span></span>|<span data-ttu-id="b7c68-109">Если параметр имеет значение true, пользователи могут изменять свои сообщения;</span><span class="sxs-lookup"><span data-stu-id="b7c68-109">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="b7c68-110">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b7c68-110">allowUserDeleteMessages</span></span>|<span data-ttu-id="b7c68-111">Логический</span><span class="sxs-lookup"><span data-stu-id="b7c68-111">Boolean</span></span>|<span data-ttu-id="b7c68-112">Если параметр имеет значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="b7c68-112">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="b7c68-113">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b7c68-113">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="b7c68-114">Логический</span><span class="sxs-lookup"><span data-stu-id="b7c68-114">Boolean</span></span>|<span data-ttu-id="b7c68-115">Если параметр имеет значение true, владельцы могут удалять все сообщения.</span><span class="sxs-lookup"><span data-stu-id="b7c68-115">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="b7c68-116">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="b7c68-116">allowTeamMentions</span></span>|<span data-ttu-id="b7c68-117">Логический</span><span class="sxs-lookup"><span data-stu-id="b7c68-117">Boolean</span></span>|<span data-ttu-id="b7c68-118">Если задано значение true, допускаются упоминания @team.</span><span class="sxs-lookup"><span data-stu-id="b7c68-118">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="b7c68-119">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="b7c68-119">allowChannelMentions</span></span>|<span data-ttu-id="b7c68-120">Логический</span><span class="sxs-lookup"><span data-stu-id="b7c68-120">Boolean</span></span>|<span data-ttu-id="b7c68-121">Если задано значение true, допускаются упоминания @channel.</span><span class="sxs-lookup"><span data-stu-id="b7c68-121">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7c68-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7c68-122">JSON representation</span></span>

<span data-ttu-id="b7c68-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7c68-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
