---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
ms.openlocfilehash: aff5abd69297cd466027c1a614b2609697c00ce6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806841"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="0d27f-103">Тип ресурса meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="0d27f-103">meetingTimeSuggestionsResult resource type</span></span>

> <span data-ttu-id="0d27f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d27f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d27f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d27f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d27f-106">Коллекция предложений (если они есть) или причина их отсутствия.</span><span class="sxs-lookup"><span data-stu-id="0d27f-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="0d27f-107">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="0d27f-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="0d27f-108">**Значение emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="0d27f-108">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="0d27f-109">**Причины**</span><span class="sxs-lookup"><span data-stu-id="0d27f-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="0d27f-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="0d27f-110">attendeesUnavailable</span></span> | <span data-ttu-id="0d27f-111">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог [достоверности собрания](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="0d27f-111">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="0d27f-112">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="0d27f-112">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="0d27f-p102">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="0d27f-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="0d27f-115">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="0d27f-115">locationsUnavailable</span></span> | <span data-ttu-id="0d27f-116">Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок.</span><span class="sxs-lookup"><span data-stu-id="0d27f-116">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="0d27f-117">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="0d27f-117">organizerUnavailable</span></span> | <span data-ttu-id="0d27f-118">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="0d27f-118">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="0d27f-119">unknown</span><span class="sxs-lookup"><span data-stu-id="0d27f-119">unknown</span></span> | <span data-ttu-id="0d27f-120">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="0d27f-120">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d27f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d27f-121">JSON representation</span></span>

<span data-ttu-id="0d27f-122">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d27f-122">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0d27f-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d27f-123">Properties</span></span>
| <span data-ttu-id="0d27f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d27f-124">Property</span></span>     | <span data-ttu-id="0d27f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0d27f-125">Type</span></span>   |<span data-ttu-id="0d27f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0d27f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d27f-127">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="0d27f-127">emptySuggestionsReason</span></span>|<span data-ttu-id="0d27f-128">String</span><span class="sxs-lookup"><span data-stu-id="0d27f-128">String</span></span>|<span data-ttu-id="0d27f-p103">Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`. Строка для этого свойства остается пустой, если свойство **meetingTimeSuggestions** включает предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="0d27f-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="0d27f-132">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="0d27f-132">meetingTimeSuggestions</span></span>|<span data-ttu-id="0d27f-133">Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="0d27f-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="0d27f-134">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="0d27f-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
