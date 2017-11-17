# <a name="reminder-resource-type"></a><span data-ttu-id="e5b36-101">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="e5b36-101">reminder resource type</span></span>



## <a name="properties"></a><span data-ttu-id="e5b36-102">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5b36-102">Properties</span></span>
| <span data-ttu-id="e5b36-103">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5b36-103">Property</span></span>     | <span data-ttu-id="e5b36-104">Тип</span><span class="sxs-lookup"><span data-stu-id="e5b36-104">Type</span></span>   |<span data-ttu-id="e5b36-105">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b36-105">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5b36-106">changeKey</span><span class="sxs-lookup"><span data-stu-id="e5b36-106">changeKey</span></span>|<span data-ttu-id="e5b36-107">String</span><span class="sxs-lookup"><span data-stu-id="e5b36-107">String</span></span>|<span data-ttu-id="e5b36-p101">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="e5b36-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="e5b36-111">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="e5b36-111">eventEndTime</span></span>|[<span data-ttu-id="e5b36-112">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5b36-112">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e5b36-113">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="e5b36-113">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="e5b36-114">eventId</span><span class="sxs-lookup"><span data-stu-id="e5b36-114">eventId</span></span>|<span data-ttu-id="e5b36-115">String</span><span class="sxs-lookup"><span data-stu-id="e5b36-115">String</span></span>|<span data-ttu-id="e5b36-p102">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5b36-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="e5b36-118">eventLocation</span><span class="sxs-lookup"><span data-stu-id="e5b36-118">eventLocation</span></span>|[<span data-ttu-id="e5b36-119">Location</span><span class="sxs-lookup"><span data-stu-id="e5b36-119">Location</span></span>](location.md)|<span data-ttu-id="e5b36-120">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="e5b36-120">The location of the event.</span></span>|
|<span data-ttu-id="e5b36-121">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="e5b36-121">eventStartTime</span></span>|[<span data-ttu-id="e5b36-122">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5b36-122">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e5b36-123">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="e5b36-123">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="e5b36-124">eventSubject</span><span class="sxs-lookup"><span data-stu-id="e5b36-124">eventSubject</span></span>|<span data-ttu-id="e5b36-125">String</span><span class="sxs-lookup"><span data-stu-id="e5b36-125">String</span></span>|<span data-ttu-id="e5b36-126">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="e5b36-126">The text of the event's subject line.</span></span>|
|<span data-ttu-id="e5b36-127">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="e5b36-127">eventWebLink</span></span>|<span data-ttu-id="e5b36-128">String</span><span class="sxs-lookup"><span data-stu-id="e5b36-128">String</span></span>|<span data-ttu-id="e5b36-129">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="e5b36-129">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="e5b36-p103">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="e5b36-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="e5b36-132">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="e5b36-132">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="e5b36-133">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="e5b36-133">reminderFireTime</span></span>|[<span data-ttu-id="e5b36-134">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5b36-134">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e5b36-135">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="e5b36-135">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5b36-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5b36-136">JSON representation</span></span>

<span data-ttu-id="e5b36-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5b36-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->