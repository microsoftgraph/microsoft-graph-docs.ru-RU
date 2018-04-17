# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="628ac-101">Тип ресурса daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="628ac-101">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="628ac-102">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-102">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="628ac-103">Допустим, для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="628ac-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="628ac-104">**bias** — 300;</span><span class="sxs-lookup"><span data-stu-id="628ac-104">**bias** is 300</span></span>
- <span data-ttu-id="628ac-105">**daylightBias** — -100;</span><span class="sxs-lookup"><span data-stu-id="628ac-105">**daylightBias** is -100</span></span>
- <span data-ttu-id="628ac-106">**dayOccurrence** — 4;</span><span class="sxs-lookup"><span data-stu-id="628ac-106">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="628ac-107">**dayOfWeek** — "sunday";</span><span class="sxs-lookup"><span data-stu-id="628ac-107">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="628ac-108">**month** — 5;</span><span class="sxs-lookup"><span data-stu-id="628ac-108">**month** is 5</span></span>
- <span data-ttu-id="628ac-109">**time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут.</span><span class="sxs-lookup"><span data-stu-id="628ac-109">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="628ac-110">Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.</span><span class="sxs-lookup"><span data-stu-id="628ac-110">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="628ac-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="628ac-111">Properties</span></span>
| <span data-ttu-id="628ac-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="628ac-112">Property</span></span>     | <span data-ttu-id="628ac-113">Тип</span><span class="sxs-lookup"><span data-stu-id="628ac-113">Type</span></span>   |<span data-ttu-id="628ac-114">Описание</span><span class="sxs-lookup"><span data-stu-id="628ac-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="628ac-115">daylightBias</span><span class="sxs-lookup"><span data-stu-id="628ac-115">daylightBias</span></span> | <span data-ttu-id="628ac-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="628ac-116">Edm.Int32</span></span> | <span data-ttu-id="628ac-117">Смещение летнего времени относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="628ac-117">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="628ac-118">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="628ac-118">This value is in points.</span></span>  |
| <span data-ttu-id="628ac-119">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="628ac-119">dayOccurrence</span></span> | <span data-ttu-id="628ac-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="628ac-120">Edm.Int32</span></span> | <span data-ttu-id="628ac-121">Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-121">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="628ac-122">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="628ac-122">dayOfWeek</span></span> | <span data-ttu-id="628ac-123">строка</span><span class="sxs-lookup"><span data-stu-id="628ac-123">string</span></span> | <span data-ttu-id="628ac-124">Представляет день недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-124">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="628ac-125">month</span><span class="sxs-lookup"><span data-stu-id="628ac-125">month</span></span> | <span data-ttu-id="628ac-126">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="628ac-126">Edm.Int32</span></span> | <span data-ttu-id="628ac-127">Представляет месяц года, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-127">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="628ac-128">time</span><span class="sxs-lookup"><span data-stu-id="628ac-128">time</span></span> | <span data-ttu-id="628ac-129">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="628ac-129">Edm.TimeOfDay</span></span> | <span data-ttu-id="628ac-130">Представляет время суток, когда происходит переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-130">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="628ac-131">year</span><span class="sxs-lookup"><span data-stu-id="628ac-131">year</span></span> | <span data-ttu-id="628ac-132">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="628ac-132">Edm.Int32</span></span> | <span data-ttu-id="628ac-133">Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="628ac-133">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="628ac-134">Например, значение 0 указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="628ac-134">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="628ac-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="628ac-135">JSON representation</span></span>

<span data-ttu-id="628ac-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="628ac-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->