# <a name="workinghours-resource-type"></a><span data-ttu-id="8a8bf-101">Тип ресурса workingHours</span><span class="sxs-lookup"><span data-stu-id="8a8bf-101">workingHours resource type</span></span>

<span data-ttu-id="8a8bf-102">Представляет дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-102">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="8a8bf-103">Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-103">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="8a8bf-104">Вы можете [получать](../api/user_get_mailboxsettings.md#request-3) и [задавать](../api/user_update_mailboxsettings.md#request-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxSettings.md).</span><span class="sxs-lookup"><span data-stu-id="8a8bf-104">You can [get](../api/user_get_mailboxsettings.md#request-3) and [set](../api/user_update_mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxSettings.md).</span></span> 

<span data-ttu-id="8a8bf-105">Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-105">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="8a8bf-106">Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-106">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="8a8bf-107">Для клиента Outlook</span><span class="sxs-lookup"><span data-stu-id="8a8bf-107">You can set the Outlook client</span></span>  
<span data-ttu-id="8a8bf-108">можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-108">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="8a8bf-109">Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-109">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="8a8bf-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a8bf-110">Properties</span></span>
| <span data-ttu-id="8a8bf-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a8bf-111">Property</span></span>     | <span data-ttu-id="8a8bf-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8a8bf-112">Type</span></span>   |<span data-ttu-id="8a8bf-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8a8bf-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a8bf-114">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="8a8bf-114">daysOfWeek</span></span> | <span data-ttu-id="8a8bf-115">Коллекция dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="8a8bf-115">dayOfWeek collection</span></span> | <span data-ttu-id="8a8bf-116">Дни недели, в которые работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-116">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="8a8bf-117">startTime</span><span class="sxs-lookup"><span data-stu-id="8a8bf-117">startTime</span></span> | <span data-ttu-id="8a8bf-118">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8a8bf-118">Edm.TimeOfDay</span></span> | <span data-ttu-id="8a8bf-119">Время дня, в которое пользователь начинает работать.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-119">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="8a8bf-120">endTime</span><span class="sxs-lookup"><span data-stu-id="8a8bf-120">endTime</span></span> | <span data-ttu-id="8a8bf-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8a8bf-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="8a8bf-122">Время дня, в которое пользователь заканчивает работать.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-122">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="8a8bf-123">timeZone</span><span class="sxs-lookup"><span data-stu-id="8a8bf-123">timeZone</span></span> | [<span data-ttu-id="8a8bf-124">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="8a8bf-124">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="8a8bf-125">Часовой пояс, к которому относится рабочее время.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-125">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a8bf-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a8bf-126">JSON representation</span></span>

<span data-ttu-id="8a8bf-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->