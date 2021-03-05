---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение собрания, которое включает сведения, такие как время собрания, вероятность посещения, индивидуальный '
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5340fa9912ecb183dda8603d4b3ce4bbf6d70e8d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474703"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="f68b3-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="f68b3-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="f68b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f68b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f68b3-105">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-105">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f68b3-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f68b3-106">JSON representation</span></span>

<span data-ttu-id="f68b3-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f68b3-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f68b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f68b3-108">Properties</span></span>
| <span data-ttu-id="f68b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f68b3-109">Property</span></span>     | <span data-ttu-id="f68b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f68b3-110">Type</span></span>   |<span data-ttu-id="f68b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f68b3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f68b3-112">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="f68b3-112">attendeeAvailability</span></span>|<span data-ttu-id="f68b3-113">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="f68b3-113">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="f68b3-114">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-114">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="f68b3-115">confidence</span><span class="sxs-lookup"><span data-stu-id="f68b3-115">confidence</span></span>|<span data-ttu-id="f68b3-116">Double</span><span class="sxs-lookup"><span data-stu-id="f68b3-116">Double</span></span>|<span data-ttu-id="f68b3-117">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="f68b3-117">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="f68b3-118">locations</span><span class="sxs-lookup"><span data-stu-id="f68b3-118">locations</span></span>|<span data-ttu-id="f68b3-119">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="f68b3-119">[location](location.md) collection</span></span>|<span data-ttu-id="f68b3-120">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-120">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="f68b3-121">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="f68b3-121">meetingTimeSlot</span></span>|[<span data-ttu-id="f68b3-122">timeSlot</span><span class="sxs-lookup"><span data-stu-id="f68b3-122">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="f68b3-123">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-123">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="f68b3-124">порядок</span><span class="sxs-lookup"><span data-stu-id="f68b3-124">order</span></span>|<span data-ttu-id="f68b3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f68b3-125">Int32</span></span>|<span data-ttu-id="f68b3-126">Порядок предложений по времени собраний, отсортироваться по их вычисляемой уверенности от высокого до низкого, а затем по хронологии, если есть предложения с той же уверенностью.</span><span class="sxs-lookup"><span data-stu-id="f68b3-126">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="f68b3-127">organisAvailability</span><span class="sxs-lookup"><span data-stu-id="f68b3-127">organizerAvailability</span></span>|<span data-ttu-id="f68b3-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f68b3-128">freeBusyStatus</span></span>| <span data-ttu-id="f68b3-129">Доступность организатора собрания для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-129">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="f68b3-130">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f68b3-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="f68b3-131">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="f68b3-131">suggestionReason</span></span>|<span data-ttu-id="f68b3-132">String</span><span class="sxs-lookup"><span data-stu-id="f68b3-132">String</span></span>|<span data-ttu-id="f68b3-133">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="f68b3-133">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

