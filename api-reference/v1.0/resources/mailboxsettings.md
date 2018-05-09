# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="d64b4-101">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="d64b4-101">mailboxSettings resource type</span></span>

<span data-ttu-id="d64b4-102">Параметры основного параметра вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="d64b4-102">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="d64b4-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="d64b4-103">Properties</span></span>
| <span data-ttu-id="d64b4-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="d64b4-104">Property</span></span>     | <span data-ttu-id="d64b4-105">Тип</span><span class="sxs-lookup"><span data-stu-id="d64b4-105">Type</span></span>   |<span data-ttu-id="d64b4-106">Описание</span><span class="sxs-lookup"><span data-stu-id="d64b4-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d64b4-107">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="d64b4-107">archiveFolder</span></span>|<span data-ttu-id="d64b4-108">string</span><span class="sxs-lookup"><span data-stu-id="d64b4-108">string</span></span>|<span data-ttu-id="d64b4-109">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="d64b4-109">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="d64b4-110">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="d64b4-110">automaticRepliesSetting</span></span>|[<span data-ttu-id="d64b4-111">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="d64b4-111">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="d64b4-112">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="d64b4-112">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="d64b4-113">language</span><span class="sxs-lookup"><span data-stu-id="d64b4-113">language</span></span>|[<span data-ttu-id="d64b4-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d64b4-114">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="d64b4-115">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="d64b4-115">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="d64b4-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="d64b4-116">timeZone</span></span>|<span data-ttu-id="d64b4-117">string</span><span class="sxs-lookup"><span data-stu-id="d64b4-117">string</span></span>|<span data-ttu-id="d64b4-118">Часовой пояс почтового ящика пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d64b4-118">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="d64b4-119">workingHours</span><span class="sxs-lookup"><span data-stu-id="d64b4-119">workingHours</span></span>|[<span data-ttu-id="d64b4-120">workingHours</span><span class="sxs-lookup"><span data-stu-id="d64b4-120">workingHours</span></span>](workinghours.md)|<span data-ttu-id="d64b4-121">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="d64b4-121">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d64b4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d64b4-122">JSON representation</span></span>

<span data-ttu-id="d64b4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d64b4-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->