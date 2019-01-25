---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 9d64fe43ac65e3366975b3981053b6d163d41522
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510822"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="50a46-103">Тип ресурса meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="50a46-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a46-104">Коллекция предложений (если они есть) или причина их отсутствия.</span><span class="sxs-lookup"><span data-stu-id="50a46-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="50a46-105">Ниже представлены возможные причины, по которым метод findMeetingTimes может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="50a46-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="50a46-106">Значение emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="50a46-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="50a46-107">Причины</span><span class="sxs-lookup"><span data-stu-id="50a46-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="50a46-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="50a46-108">attendeesUnavailable</span></span> | <span data-ttu-id="50a46-109">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог [достоверности собрания](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="50a46-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="50a46-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="50a46-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="50a46-p101">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="50a46-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="50a46-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="50a46-113">locationsUnavailable</span></span> | <span data-ttu-id="50a46-114">Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок.</span><span class="sxs-lookup"><span data-stu-id="50a46-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="50a46-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="50a46-115">organizerUnavailable</span></span> | <span data-ttu-id="50a46-116">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="50a46-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="50a46-117">unknown</span><span class="sxs-lookup"><span data-stu-id="50a46-117">unknown</span></span> | <span data-ttu-id="50a46-118">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="50a46-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50a46-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50a46-119">JSON representation</span></span>

<span data-ttu-id="50a46-120">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="50a46-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="50a46-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="50a46-121">Properties</span></span>
| <span data-ttu-id="50a46-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="50a46-122">Property</span></span>     | <span data-ttu-id="50a46-123">Тип</span><span class="sxs-lookup"><span data-stu-id="50a46-123">Type</span></span>   |<span data-ttu-id="50a46-124">Описание</span><span class="sxs-lookup"><span data-stu-id="50a46-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50a46-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="50a46-125">emptySuggestionsReason</span></span>|<span data-ttu-id="50a46-126">String</span><span class="sxs-lookup"><span data-stu-id="50a46-126">String</span></span>|<span data-ttu-id="50a46-p102">Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`. Строка для этого свойства остается пустой, если свойство **meetingTimeSuggestions** включает предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="50a46-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="50a46-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="50a46-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="50a46-131">Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="50a46-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="50a46-132">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="50a46-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestionsresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
