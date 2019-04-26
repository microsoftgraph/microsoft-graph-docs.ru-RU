---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений собраний, если таковая существует, и причина в отсутствии.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1e3fb99e7675544f39b359abd226875a7721e287
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342312"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="0515f-103">Тип ресурса meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="0515f-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0515f-104">Коллекция предложений собраний, если таковая существует, и причина в отсутствии.</span><span class="sxs-lookup"><span data-stu-id="0515f-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="0515f-105">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="0515f-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="0515f-106">**Значение emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="0515f-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="0515f-107">**Причины**</span><span class="sxs-lookup"><span data-stu-id="0515f-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="0515f-108">Аттендисунаваилабле</span><span class="sxs-lookup"><span data-stu-id="0515f-108">attendeesUnavailable</span></span> | <span data-ttu-id="0515f-109">Все сведения о доступности участников известны, но недостаточно участников для достижения порогового значения, которое составляет [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) 50% по умолчанию для любого периода времени.</span><span class="sxs-lookup"><span data-stu-id="0515f-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="0515f-110">Аттендисунаваилаблеорункновн</span><span class="sxs-lookup"><span data-stu-id="0515f-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="0515f-p101">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="0515f-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="0515f-113">Локатионсунаваилабле</span><span class="sxs-lookup"><span data-stu-id="0515f-113">locationsUnavailable</span></span> | <span data-ttu-id="0515f-114">Для свойства **Required** параметра **locationConstraint** задано значение true, но в вычисляемых интервалах времени нет доступных расположений.</span><span class="sxs-lookup"><span data-stu-id="0515f-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="0515f-115">Организерунаваилабле</span><span class="sxs-lookup"><span data-stu-id="0515f-115">organizerUnavailable</span></span> | <span data-ttu-id="0515f-116">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="0515f-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="0515f-117">unknown</span><span class="sxs-lookup"><span data-stu-id="0515f-117">unknown</span></span> | <span data-ttu-id="0515f-118">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="0515f-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0515f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0515f-119">JSON representation</span></span>

<span data-ttu-id="0515f-120">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0515f-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0515f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0515f-121">Properties</span></span>
| <span data-ttu-id="0515f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0515f-122">Property</span></span>     | <span data-ttu-id="0515f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0515f-123">Type</span></span>   |<span data-ttu-id="0515f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0515f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0515f-125">Емптисугжестионсреасон</span><span class="sxs-lookup"><span data-stu-id="0515f-125">emptySuggestionsReason</span></span>|<span data-ttu-id="0515f-126">String</span><span class="sxs-lookup"><span data-stu-id="0515f-126">String</span></span>|<span data-ttu-id="0515f-127">Причина отсутствия предложений в результатах.</span><span class="sxs-lookup"><span data-stu-id="0515f-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="0515f-128">Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0515f-128">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="0515f-129">Это свойство представляет собой пустую строку, если в свойстве **митингтимесугжестионс** есть предложения о собраниях.</span><span class="sxs-lookup"><span data-stu-id="0515f-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="0515f-130">Митингтимесугжестионс</span><span class="sxs-lookup"><span data-stu-id="0515f-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="0515f-131">Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="0515f-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="0515f-132">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="0515f-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
