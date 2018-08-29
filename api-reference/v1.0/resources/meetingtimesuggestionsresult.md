# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="36155-101">Тип ресурса meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="36155-101">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="36155-102">Коллекция предложений встречи (если они есть) или причина их отсутствия.</span><span class="sxs-lookup"><span data-stu-id="36155-102">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="36155-103">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user_findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="36155-103">The following are the possible reasons that [findMeetingTimes](../api/user_findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="36155-104">**Значение emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="36155-104">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="36155-105">**Причины**</span><span class="sxs-lookup"><span data-stu-id="36155-105">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="36155-106">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="36155-106">attendeesUnavailable</span></span> | <span data-ttu-id="36155-107">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог [достоверности собрания](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="36155-107">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="36155-108">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="36155-108">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="36155-p101">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="36155-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="36155-111">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="36155-111">locationsUnavailable</span></span> | <span data-ttu-id="36155-112">Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступного местоположения.</span><span class="sxs-lookup"><span data-stu-id="36155-112">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="36155-113">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="36155-113">organizerUnavailable</span></span> | <span data-ttu-id="36155-114">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="36155-114">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="36155-115">unknown</span><span class="sxs-lookup"><span data-stu-id="36155-115">unknown</span></span> | <span data-ttu-id="36155-116">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="36155-116">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36155-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36155-117">JSON representation</span></span>

<span data-ttu-id="36155-118">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="36155-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="36155-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="36155-119">Properties</span></span>
| <span data-ttu-id="36155-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="36155-120">Property</span></span>     | <span data-ttu-id="36155-121">Тип</span><span class="sxs-lookup"><span data-stu-id="36155-121">Type</span></span>   |<span data-ttu-id="36155-122">Описание</span><span class="sxs-lookup"><span data-stu-id="36155-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36155-123">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="36155-123">emptySuggestionsReason</span></span>|<span data-ttu-id="36155-124">String</span><span class="sxs-lookup"><span data-stu-id="36155-124">String</span></span>|<span data-ttu-id="36155-125">Причина для того, чтобы не возвращать какие-либо предложения встреч.</span><span class="sxs-lookup"><span data-stu-id="36155-125">A reason for not returning any meeting suggestions. Possible values are: , , , , or .</span></span> <span data-ttu-id="36155-126">Допустимые значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` или `unknown`.</span><span class="sxs-lookup"><span data-stu-id="36155-126">The possible values are `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, , , , , , , , or `unknown`.</span></span> <span data-ttu-id="36155-127">Это свойство — пустая строка, если свойство **meetingTimeSuggestions** включает какое-либо предложение встречи.</span><span class="sxs-lookup"><span data-stu-id="36155-127">A reason for not returning any meeting suggestions. Possible values are: , , , , or . This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="36155-128">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="36155-128">meetingTimeSuggestions</span></span>|<span data-ttu-id="36155-129">Коллекция [meetingTimeSuggestion](meetingTimeSuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="36155-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span></span>|<span data-ttu-id="36155-130">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="36155-130">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->