---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение о собрании, которое включает такие сведения, как время собрания, вероятность посещения, Индивидуальная '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4c5a4cb4d094e7fd7fe9b0e56227a556c6e5b5d1
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936264"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="ba035-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="ba035-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="ba035-104">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba035-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba035-105">JSON representation</span></span>

<span data-ttu-id="ba035-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ba035-106">Here is a JSON representation of the resource</span></span>

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
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="ba035-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba035-107">Properties</span></span>
| <span data-ttu-id="ba035-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba035-108">Property</span></span>     | <span data-ttu-id="ba035-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba035-109">Type</span></span>   |<span data-ttu-id="ba035-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba035-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba035-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="ba035-111">attendeeAvailability</span></span>|<span data-ttu-id="ba035-112">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="ba035-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="ba035-113">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="ba035-114">confidence</span><span class="sxs-lookup"><span data-stu-id="ba035-114">confidence</span></span>|<span data-ttu-id="ba035-115">Double</span><span class="sxs-lookup"><span data-stu-id="ba035-115">Double</span></span>|<span data-ttu-id="ba035-116">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="ba035-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="ba035-117">locations</span><span class="sxs-lookup"><span data-stu-id="ba035-117">locations</span></span>|<span data-ttu-id="ba035-118">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="ba035-118">[location](location.md) collection</span></span>|<span data-ttu-id="ba035-119">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="ba035-120">Митингтимеслот</span><span class="sxs-lookup"><span data-stu-id="ba035-120">meetingTimeSlot</span></span>|[<span data-ttu-id="ba035-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ba035-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="ba035-122">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="ba035-123">порядке</span><span class="sxs-lookup"><span data-stu-id="ba035-123">order</span></span>|<span data-ttu-id="ba035-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ba035-124">Int32</span></span>|<span data-ttu-id="ba035-125">Порядок предложений по времени собраний, отсортированных по их вычисленному значению, от высокого до невысокой, затем по чронологи при наличии предложений с одинаковым уровнем достоверности.</span><span class="sxs-lookup"><span data-stu-id="ba035-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="ba035-126">Организераваилабилити</span><span class="sxs-lookup"><span data-stu-id="ba035-126">organizerAvailability</span></span>|<span data-ttu-id="ba035-127">Фрибусистатус</span><span class="sxs-lookup"><span data-stu-id="ba035-127">freeBusyStatus</span></span>| <span data-ttu-id="ba035-128">Доступность организатора собрания для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-128">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="ba035-129">Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="ba035-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="ba035-130">Suggestionreason объяснение</span><span class="sxs-lookup"><span data-stu-id="ba035-130">suggestionReason</span></span>|<span data-ttu-id="ba035-131">String</span><span class="sxs-lookup"><span data-stu-id="ba035-131">String</span></span>|<span data-ttu-id="ba035-132">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ba035-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
