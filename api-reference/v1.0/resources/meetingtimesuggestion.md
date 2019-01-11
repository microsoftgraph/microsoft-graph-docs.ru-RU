---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложения о собрании, который содержит сведения, например, время собрания, вероятность присутствия, отдельных '
localization_priority: Normal
ms.openlocfilehash: d1cca365c66c114063fbf859e241a5d9a81303e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845999"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="fcb7a-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="fcb7a-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="fcb7a-104">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcb7a-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fcb7a-105">JSON representation</span></span>

<span data-ttu-id="fcb7a-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fcb7a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcb7a-107">Properties</span></span>
| <span data-ttu-id="fcb7a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcb7a-108">Property</span></span>     | <span data-ttu-id="fcb7a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fcb7a-109">Type</span></span>   |<span data-ttu-id="fcb7a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fcb7a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcb7a-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="fcb7a-111">attendeeAvailability</span></span>|<span data-ttu-id="fcb7a-112">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="fcb7a-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="fcb7a-113">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="fcb7a-114">confidence</span><span class="sxs-lookup"><span data-stu-id="fcb7a-114">confidence</span></span>|<span data-ttu-id="fcb7a-115">Double</span><span class="sxs-lookup"><span data-stu-id="fcb7a-115">Double</span></span>|<span data-ttu-id="fcb7a-116">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="fcb7a-117">locations</span><span class="sxs-lookup"><span data-stu-id="fcb7a-117">locations</span></span>|<span data-ttu-id="fcb7a-118">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="fcb7a-118">[location](location.md) collection</span></span>|<span data-ttu-id="fcb7a-119">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="fcb7a-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="fcb7a-120">meetingTimeSlot</span></span>|[<span data-ttu-id="fcb7a-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="fcb7a-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="fcb7a-122">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="fcb7a-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="fcb7a-123">organizerAvailability</span></span>|<span data-ttu-id="fcb7a-124">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="fcb7a-124">freeBusyStatus</span></span>| <span data-ttu-id="fcb7a-125">Доступность Организатор собрания для этого предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-125">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="fcb7a-126">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-126">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="fcb7a-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="fcb7a-127">suggestionReason</span></span>|<span data-ttu-id="fcb7a-128">String</span><span class="sxs-lookup"><span data-stu-id="fcb7a-128">String</span></span>|<span data-ttu-id="fcb7a-129">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
