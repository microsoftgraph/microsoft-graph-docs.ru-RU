---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение о собрании, которое включает такие сведения, как время собрания, вероятность посещения, Индивидуальная '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d24220b43573aff655d7af9b4a60b76322de60ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522717"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="bd6ac-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="bd6ac-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="bd6ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd6ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6ac-105">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-105">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd6ac-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd6ac-106">JSON representation</span></span>

<span data-ttu-id="bd6ac-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-107">Here is a JSON representation of the resource</span></span>

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
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="bd6ac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd6ac-108">Properties</span></span>
| <span data-ttu-id="bd6ac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd6ac-109">Property</span></span>     | <span data-ttu-id="bd6ac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd6ac-110">Type</span></span>   |<span data-ttu-id="bd6ac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6ac-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd6ac-112">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="bd6ac-112">attendeeAvailability</span></span>|<span data-ttu-id="bd6ac-113">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="bd6ac-113">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="bd6ac-114">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-114">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="bd6ac-115">confidence</span><span class="sxs-lookup"><span data-stu-id="bd6ac-115">confidence</span></span>|<span data-ttu-id="bd6ac-116">Double</span><span class="sxs-lookup"><span data-stu-id="bd6ac-116">Double</span></span>|<span data-ttu-id="bd6ac-117">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-117">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="bd6ac-118">locations</span><span class="sxs-lookup"><span data-stu-id="bd6ac-118">locations</span></span>|<span data-ttu-id="bd6ac-119">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="bd6ac-119">[location](location.md) collection</span></span>|<span data-ttu-id="bd6ac-120">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-120">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="bd6ac-121">митингтимеслот</span><span class="sxs-lookup"><span data-stu-id="bd6ac-121">meetingTimeSlot</span></span>|[<span data-ttu-id="bd6ac-122">timeSlot</span><span class="sxs-lookup"><span data-stu-id="bd6ac-122">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="bd6ac-123">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-123">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="bd6ac-124">порядке</span><span class="sxs-lookup"><span data-stu-id="bd6ac-124">order</span></span>|<span data-ttu-id="bd6ac-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bd6ac-125">Int32</span></span>|<span data-ttu-id="bd6ac-126">Порядок предложений по времени собраний, отсортированных по их вычисленному значению, от высокого до невысокой, затем по чронологи при наличии предложений с одинаковым уровнем достоверности.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-126">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="bd6ac-127">организераваилабилити</span><span class="sxs-lookup"><span data-stu-id="bd6ac-127">organizerAvailability</span></span>|<span data-ttu-id="bd6ac-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="bd6ac-128">freeBusyStatus</span></span>| <span data-ttu-id="bd6ac-p101">Доступность организатора собрания для этого варианта собрания. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="bd6ac-131">Suggestionreason объяснение</span><span class="sxs-lookup"><span data-stu-id="bd6ac-131">suggestionReason</span></span>|<span data-ttu-id="bd6ac-132">String</span><span class="sxs-lookup"><span data-stu-id="bd6ac-132">String</span></span>|<span data-ttu-id="bd6ac-133">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="bd6ac-133">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
