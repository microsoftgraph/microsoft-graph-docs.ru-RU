---
title: Тип ресурса meetingTimeCandidatesResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: e60c0092ca5724e4019a4c3f75f1239a0e7e9c0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507518"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="b0122-103">Тип ресурса meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="b0122-103">meetingTimeCandidatesResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0122-104">Коллекция предложений (если они есть) или причина их отсутствия.</span><span class="sxs-lookup"><span data-stu-id="b0122-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="b0122-105">Ниже представлены возможные причины, по которым метод findMeetingTimes может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="b0122-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="b0122-106">**значение emptySuggestionsHint**</span><span class="sxs-lookup"><span data-stu-id="b0122-106">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="b0122-107">Причины</span><span class="sxs-lookup"><span data-stu-id="b0122-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="b0122-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="b0122-108">attendeesUnavailable</span></span> | <span data-ttu-id="b0122-109">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог достоверности собрания (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="b0122-109">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="b0122-110">Это значение превышено основано на участников состояния занятости для предложенного собрания периода времени со статусом бесплатную участника, соответствующий 100% вероятность присутствия, состояние Нет 50% и % 0 состояние «занят».</span><span class="sxs-lookup"><span data-stu-id="b0122-110">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="b0122-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="b0122-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="b0122-p102">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="b0122-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="b0122-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="b0122-114">locationsUnavailable</span></span> | <span data-ttu-id="b0122-115">Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок.</span><span class="sxs-lookup"><span data-stu-id="b0122-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="b0122-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="b0122-116">organizerUnavailable</span></span> | <span data-ttu-id="b0122-117">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="b0122-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="b0122-118">unknown</span><span class="sxs-lookup"><span data-stu-id="b0122-118">unknown</span></span> | <span data-ttu-id="b0122-119">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="b0122-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0122-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0122-120">JSON representation</span></span>

<span data-ttu-id="b0122-121">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b0122-121">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b0122-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0122-122">Properties</span></span>
| <span data-ttu-id="b0122-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0122-123">Property</span></span>     | <span data-ttu-id="b0122-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b0122-124">Type</span></span>   |<span data-ttu-id="b0122-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b0122-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0122-126">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="b0122-126">emptySuggestionsHint</span></span>|<span data-ttu-id="b0122-127">String</span><span class="sxs-lookup"><span data-stu-id="b0122-127">String</span></span>|<span data-ttu-id="b0122-p103">Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b0122-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="b0122-130">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="b0122-130">meetingTimeSlots</span></span>|<span data-ttu-id="b0122-131">[meetingTimeCandidate](meetingtimecandidate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b0122-131">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="b0122-132">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="b0122-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidatesresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
