# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="ba212-101">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="ba212-101">teamGuestSettings resource type</span></span>



<span data-ttu-id="ba212-102">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="ba212-102">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba212-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba212-103">Properties</span></span>
| <span data-ttu-id="ba212-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba212-104">Property</span></span>     | <span data-ttu-id="ba212-105">Тип</span><span class="sxs-lookup"><span data-stu-id="ba212-105">Type</span></span>   |<span data-ttu-id="ba212-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ba212-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba212-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ba212-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ba212-108">Логический</span><span class="sxs-lookup"><span data-stu-id="ba212-108">Boolean</span></span>|<span data-ttu-id="ba212-109">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="ba212-109">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="ba212-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ba212-110">allowDeleteChannels</span></span>|<span data-ttu-id="ba212-111">Логический</span><span class="sxs-lookup"><span data-stu-id="ba212-111">Boolean</span></span>|<span data-ttu-id="ba212-112">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="ba212-112">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba212-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba212-113">JSON representation</span></span>

<span data-ttu-id="ba212-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba212-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
