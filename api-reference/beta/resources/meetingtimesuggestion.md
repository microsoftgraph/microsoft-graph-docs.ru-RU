---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложения о собрании, который содержит сведения, например, время собрания, вероятность присутствия, отдельных '
localization_priority: Normal
ms.openlocfilehash: a38a971bb43fa13d8617e5fad1c4b5646bf224ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884430"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="ef79a-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="ef79a-103">meetingTimeSuggestion resource type</span></span>

> <span data-ttu-id="ef79a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef79a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef79a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef79a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef79a-106">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ef79a-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef79a-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef79a-107">JSON representation</span></span>

<span data-ttu-id="ef79a-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ef79a-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="ef79a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef79a-109">Properties</span></span>
| <span data-ttu-id="ef79a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef79a-110">Property</span></span>     | <span data-ttu-id="ef79a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ef79a-111">Type</span></span>   |<span data-ttu-id="ef79a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ef79a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef79a-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="ef79a-113">attendeeAvailability</span></span>|<span data-ttu-id="ef79a-114">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="ef79a-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="ef79a-115">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="ef79a-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="ef79a-116">confidence</span><span class="sxs-lookup"><span data-stu-id="ef79a-116">confidence</span></span>|<span data-ttu-id="ef79a-117">Double</span><span class="sxs-lookup"><span data-stu-id="ef79a-117">Double</span></span>|<span data-ttu-id="ef79a-118">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="ef79a-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="ef79a-119">locations</span><span class="sxs-lookup"><span data-stu-id="ef79a-119">locations</span></span>|<span data-ttu-id="ef79a-120">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="ef79a-120">[location](location.md) collection</span></span>|<span data-ttu-id="ef79a-121">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="ef79a-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="ef79a-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="ef79a-122">meetingTimeSlot</span></span>|[<span data-ttu-id="ef79a-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ef79a-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="ef79a-124">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="ef79a-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="ef79a-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="ef79a-125">organizerAvailability</span></span>|<span data-ttu-id="ef79a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="ef79a-126">String</span></span>| <span data-ttu-id="ef79a-p102">Доступность организатора собрания для этого варианта собрания. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ef79a-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="ef79a-129">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="ef79a-129">suggestionReason</span></span>|<span data-ttu-id="ef79a-130">String</span><span class="sxs-lookup"><span data-stu-id="ef79a-130">String</span></span>|<span data-ttu-id="ef79a-131">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ef79a-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
