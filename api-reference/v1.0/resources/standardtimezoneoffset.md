# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="fca61-101">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fca61-101">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="fca61-102">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fca61-102">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="fca61-103">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="fca61-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="fca61-104">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="fca61-104">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="fca61-105">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="fca61-105">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="fca61-106">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="fca61-106">**month** is 10</span></span>
- <span data-ttu-id="fca61-107">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="fca61-107">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="fca61-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fca61-108">Properties</span></span>
| <span data-ttu-id="fca61-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fca61-109">Property</span></span>     | <span data-ttu-id="fca61-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fca61-110">Type</span></span>   |<span data-ttu-id="fca61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fca61-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fca61-112">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="fca61-112">dayOccurrence</span></span> | <span data-ttu-id="fca61-113">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fca61-113">Edm.Int32</span></span> | <span data-ttu-id="fca61-114">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="fca61-114">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fca61-115">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fca61-115">dayOfWeek</span></span> | <span data-ttu-id="fca61-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fca61-116">dayOfWeek</span></span> | <span data-ttu-id="fca61-117">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fca61-117">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="fca61-118">month</span><span class="sxs-lookup"><span data-stu-id="fca61-118">month</span></span> | <span data-ttu-id="fca61-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fca61-119">Edm.Int32</span></span> | <span data-ttu-id="fca61-120">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fca61-120">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fca61-121">time</span><span class="sxs-lookup"><span data-stu-id="fca61-121">time</span></span> | <span data-ttu-id="fca61-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fca61-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="fca61-123">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fca61-123">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fca61-124">year</span><span class="sxs-lookup"><span data-stu-id="fca61-124">year</span></span> | <span data-ttu-id="fca61-125">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fca61-125">Edm.Int32</span></span> | <span data-ttu-id="fca61-126">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="fca61-126">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="fca61-127">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="fca61-127">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fca61-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fca61-128">JSON representation</span></span>

<span data-ttu-id="fca61-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fca61-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->