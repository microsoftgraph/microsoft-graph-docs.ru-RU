---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений о собраниях, если они есть, и причина, по которой их нет.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 87b4a2515ced0baf8518b11d6f5e2042211e3483
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471805"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="76168-103">Тип ресурса meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="76168-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="76168-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76168-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76168-105">Коллекция предложений о собраниях, если они есть, и причина, по которой их нет.</span><span class="sxs-lookup"><span data-stu-id="76168-105">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="76168-106">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="76168-106">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="76168-107">**Значение emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="76168-107">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="76168-108">**Причины**</span><span class="sxs-lookup"><span data-stu-id="76168-108">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="76168-109">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="76168-109">attendeesUnavailable</span></span> | <span data-ttu-id="76168-110">Доступность всех участников известна, но для достижения порога доверия к [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) собранию, который по умолчанию составляет 50% для любого периода времени, недостаточно.</span><span class="sxs-lookup"><span data-stu-id="76168-110">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="76168-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="76168-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="76168-p101">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="76168-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="76168-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="76168-114">locationsUnavailable</span></span> | <span data-ttu-id="76168-115">Свойство **isRequired** **параметра locationConstraint** указывается как true, но в расчетных интервалах времени нет расположения.</span><span class="sxs-lookup"><span data-stu-id="76168-115">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="76168-116">organisUnavailable</span><span class="sxs-lookup"><span data-stu-id="76168-116">organizerUnavailable</span></span> | <span data-ttu-id="76168-117">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="76168-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="76168-118">unknown</span><span class="sxs-lookup"><span data-stu-id="76168-118">unknown</span></span> | <span data-ttu-id="76168-119">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="76168-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76168-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76168-120">JSON representation</span></span>

<span data-ttu-id="76168-121">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="76168-121">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="76168-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="76168-122">Properties</span></span>
| <span data-ttu-id="76168-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="76168-123">Property</span></span>     | <span data-ttu-id="76168-124">Тип</span><span class="sxs-lookup"><span data-stu-id="76168-124">Type</span></span>   |<span data-ttu-id="76168-125">Описание</span><span class="sxs-lookup"><span data-stu-id="76168-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76168-126">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="76168-126">emptySuggestionsReason</span></span>|<span data-ttu-id="76168-127">String</span><span class="sxs-lookup"><span data-stu-id="76168-127">String</span></span>|<span data-ttu-id="76168-128">Причина отсутствия предложений в результатах.</span><span class="sxs-lookup"><span data-stu-id="76168-128">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="76168-129">Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="76168-129">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="76168-130">Это свойство — пустая строка, если свойство **meetingTimeSuggestions** содержит любые предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="76168-130">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="76168-131">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="76168-131">meetingTimeSuggestions</span></span>|<span data-ttu-id="76168-132">Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="76168-132">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="76168-133">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="76168-133">An array of meeting suggestions.</span></span>|

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


