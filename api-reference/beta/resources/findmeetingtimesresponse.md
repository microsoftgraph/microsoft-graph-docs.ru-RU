---
title: Тип ресурса Финдмитингтимесреспонсе
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0d52da8e5798932d4f78463d6e4bea08ecb7c793
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057417"
---
# <a name="findmeetingtimesresponse-resource-type"></a><span data-ttu-id="4feee-103">Тип ресурса Финдмитингтимесреспонсе</span><span class="sxs-lookup"><span data-stu-id="4feee-103">findMeetingTimesResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4feee-104">Коллекция предложений собраний, если таковая существует, и причина в отсутствии.</span><span class="sxs-lookup"><span data-stu-id="4feee-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="4feee-105">Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.</span><span class="sxs-lookup"><span data-stu-id="4feee-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="4feee-106">**Значение emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="4feee-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="4feee-107">**Причины**</span><span class="sxs-lookup"><span data-stu-id="4feee-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="4feee-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="4feee-108">attendeesUnavailable</span></span> | <span data-ttu-id="4feee-109">Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог [достоверности собрания](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) (значение по умолчанию — 50 %).</span><span class="sxs-lookup"><span data-stu-id="4feee-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="4feee-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="4feee-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="4feee-p101">Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="4feee-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="4feee-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="4feee-113">locationsUnavailable</span></span> | <span data-ttu-id="4feee-114">Для свойства **Required** параметра **locationConstraint** задано значение true, но в вычисляемых интервалах времени нет доступных расположений.</span><span class="sxs-lookup"><span data-stu-id="4feee-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="4feee-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="4feee-115">organizerUnavailable</span></span> | <span data-ttu-id="4feee-116">Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени.</span><span class="sxs-lookup"><span data-stu-id="4feee-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="4feee-117">unknown</span><span class="sxs-lookup"><span data-stu-id="4feee-117">unknown</span></span> | <span data-ttu-id="4feee-118">Причина отсутствия предложений неизвестна.</span><span class="sxs-lookup"><span data-stu-id="4feee-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4feee-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4feee-119">JSON representation</span></span>

<span data-ttu-id="4feee-120">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4feee-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesResponse"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="4feee-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4feee-121">Properties</span></span>
| <span data-ttu-id="4feee-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="4feee-122">Property</span></span>     | <span data-ttu-id="4feee-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4feee-123">Type</span></span>   |<span data-ttu-id="4feee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4feee-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4feee-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="4feee-125">emptySuggestionsReason</span></span>|<span data-ttu-id="4feee-126">String</span><span class="sxs-lookup"><span data-stu-id="4feee-126">String</span></span>|<span data-ttu-id="4feee-p102">Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`. Строка для этого свойства остается пустой, если свойство **meetingTimeSuggestions** включает предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="4feee-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="4feee-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="4feee-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="4feee-131">Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="4feee-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="4feee-132">Массив предложений.</span><span class="sxs-lookup"><span data-stu-id="4feee-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimesresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->