---
title: Тип ресурса meetingTimeCandidatesResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
ms.openlocfilehash: 38ca5b6be15d3cd268403f7f95645a8aaf31cf9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075529"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="06042-103">Тип ресурса meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="06042-103">meetingTimeCandidatesResult resource type</span></span>

> <span data-ttu-id="06042-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06042-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06042-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06042-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06042-106">Коллекция предложений (если они есть) или причина их отсутствия.</span><span class="sxs-lookup"><span data-stu-id="06042-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="06042-107">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="06042-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="06042-108">**значение emptySuggestionsHint**</span><span class="sxs-lookup"><span data-stu-id="06042-108">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="06042-109">**Причины**</span><span class="sxs-lookup"><span data-stu-id="06042-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="06042-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="06042-110">attendeesUnavailable</span></span> | <span data-ttu-id="06042-111">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог достоверности собрания (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="06042-111">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="06042-112">Это значение превышено основано на участников состояния занятости для предложенного собрания периода времени со статусом бесплатную участника, соответствующий 100% вероятность присутствия, состояние Нет 50% и % 0 состояние «занят».</span><span class="sxs-lookup"><span data-stu-id="06042-112">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="06042-113">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="06042-113">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="06042-p103">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="06042-p103">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="06042-116">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="06042-116">locationsUnavailable</span></span> | <span data-ttu-id="06042-117">Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок.</span><span class="sxs-lookup"><span data-stu-id="06042-117">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="06042-118">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="06042-118">organizerUnavailable</span></span> | <span data-ttu-id="06042-119">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="06042-119">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="06042-120">unknown</span><span class="sxs-lookup"><span data-stu-id="06042-120">unknown</span></span> | <span data-ttu-id="06042-121">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="06042-121">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06042-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06042-122">JSON representation</span></span>

<span data-ttu-id="06042-123">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="06042-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a><span data-ttu-id="06042-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="06042-124">Properties</span></span>
| <span data-ttu-id="06042-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="06042-125">Property</span></span>     | <span data-ttu-id="06042-126">Тип</span><span class="sxs-lookup"><span data-stu-id="06042-126">Type</span></span>   |<span data-ttu-id="06042-127">Description</span><span class="sxs-lookup"><span data-stu-id="06042-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06042-128">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="06042-128">emptySuggestionsHint</span></span>|<span data-ttu-id="06042-129">String</span><span class="sxs-lookup"><span data-stu-id="06042-129">String</span></span>|<span data-ttu-id="06042-p104">Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="06042-p104">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="06042-132">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="06042-132">meetingTimeSlots</span></span>|<span data-ttu-id="06042-133">[meetingTimeCandidate](meetingtimecandidate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="06042-133">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="06042-134">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="06042-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->