# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="390d6-101">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="390d6-101">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="390d6-p101">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="390d6-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="390d6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="390d6-104">Properties</span></span>
| <span data-ttu-id="390d6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="390d6-105">Property</span></span>     | <span data-ttu-id="390d6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="390d6-106">Type</span></span>   |<span data-ttu-id="390d6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="390d6-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="390d6-108">externalAudience</span><span class="sxs-lookup"><span data-stu-id="390d6-108">externalAudience</span></span>|<span data-ttu-id="390d6-109">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="390d6-109">externalAudienceScope values</span></span>| <span data-ttu-id="390d6-110">Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-110">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or . Possible values are: , , `Scheduled`.</span></span> <span data-ttu-id="390d6-111">Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="390d6-111">The possible values are `none`, `contactsOnly`, `all`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="390d6-112">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="390d6-112">externalReplyMessage</span></span>|<span data-ttu-id="390d6-113">строка</span><span class="sxs-lookup"><span data-stu-id="390d6-113">string</span></span>|<span data-ttu-id="390d6-114">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-114">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="390d6-115">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="390d6-115">internalReplyMessage</span></span>|<span data-ttu-id="390d6-116">строка</span><span class="sxs-lookup"><span data-stu-id="390d6-116">string</span></span>|<span data-ttu-id="390d6-117">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-117">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="390d6-118">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="390d6-118">scheduledEndDateTime</span></span>|[<span data-ttu-id="390d6-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="390d6-119">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="390d6-120">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-120">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="390d6-121">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="390d6-121">scheduledStartDateTime</span></span>|[<span data-ttu-id="390d6-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="390d6-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="390d6-123">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-123">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="390d6-124">status</span><span class="sxs-lookup"><span data-stu-id="390d6-124">status</span></span>|<span data-ttu-id="390d6-125">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="390d6-125">automaticRepliesStatus values</span></span>|<span data-ttu-id="390d6-126">Состояние конфигурации для автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="390d6-126">Configurations status for automatic replies. Possible values are: , , .</span></span> <span data-ttu-id="390d6-127">Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="390d6-127">The possible values are `disabled`, `alwaysEnabled`, `scheduled`, , , , , , , , , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="390d6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="390d6-128">JSON representation</span></span>

<span data-ttu-id="390d6-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="390d6-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
