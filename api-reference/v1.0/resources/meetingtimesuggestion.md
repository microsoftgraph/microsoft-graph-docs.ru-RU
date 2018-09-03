# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="63f83-101">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="63f83-101">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="63f83-102">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-102">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63f83-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="63f83-103">JSON representation</span></span>

<span data-ttu-id="63f83-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="63f83-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="63f83-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="63f83-105">Properties</span></span>
| <span data-ttu-id="63f83-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="63f83-106">Property</span></span>     | <span data-ttu-id="63f83-107">Тип</span><span class="sxs-lookup"><span data-stu-id="63f83-107">Type</span></span>   |<span data-ttu-id="63f83-108">Описание</span><span class="sxs-lookup"><span data-stu-id="63f83-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f83-109">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="63f83-109">attendeeAvailability</span></span>|<span data-ttu-id="63f83-110">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="63f83-110">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="63f83-111">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-111">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="63f83-112">confidence</span><span class="sxs-lookup"><span data-stu-id="63f83-112">confidence</span></span>|<span data-ttu-id="63f83-113">Double</span><span class="sxs-lookup"><span data-stu-id="63f83-113">Double</span></span>|<span data-ttu-id="63f83-114">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="63f83-114">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="63f83-115">locations</span><span class="sxs-lookup"><span data-stu-id="63f83-115">locations</span></span>|<span data-ttu-id="63f83-116">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="63f83-116">[location](location.md) collection</span></span>|<span data-ttu-id="63f83-117">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-117">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="63f83-118">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="63f83-118">meetingTimeSlot</span></span>|[<span data-ttu-id="63f83-119">timeSlot</span><span class="sxs-lookup"><span data-stu-id="63f83-119">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="63f83-120">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-120">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="63f83-121">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="63f83-121">organizerAvailability</span></span>|<span data-ttu-id="63f83-122">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="63f83-122">freeBusyStatus values</span></span>| <span data-ttu-id="63f83-123">Доступность организатора собрания для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-123">Availability of the meeting organizer for this meeting suggestion. Possible values are: , , , , , .</span></span> <span data-ttu-id="63f83-124">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="63f83-124">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="63f83-125">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="63f83-125">suggestionReason</span></span>|<span data-ttu-id="63f83-126">String (строка)</span><span class="sxs-lookup"><span data-stu-id="63f83-126">String</span></span>|<span data-ttu-id="63f83-127">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="63f83-127">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->