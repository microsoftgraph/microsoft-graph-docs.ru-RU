---
title: Тип ресурса meetingTimeCandidate
description: 'Предложения о собрании, который содержит сведения, например, время собрания, вероятность присутствия, отдельных '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 7da1240bc5bce285b041ef55ce372ba137b9d74a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523696"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="e7ab4-103">Тип ресурса meetingTimeCandidate</span><span class="sxs-lookup"><span data-stu-id="e7ab4-103">meetingTimeCandidate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7ab4-104">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7ab4-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7ab4-105">JSON representation</span></span>

<span data-ttu-id="e7ab4-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a><span data-ttu-id="e7ab4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7ab4-107">Properties</span></span>
| <span data-ttu-id="e7ab4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7ab4-108">Property</span></span>     | <span data-ttu-id="e7ab4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e7ab4-109">Type</span></span>   |<span data-ttu-id="e7ab4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e7ab4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7ab4-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e7ab4-111">attendeeAvailability</span></span>|<span data-ttu-id="e7ab4-112">Коллекция [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="e7ab4-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="e7ab4-113">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="e7ab4-114">confidence</span><span class="sxs-lookup"><span data-stu-id="e7ab4-114">confidence</span></span>|<span data-ttu-id="e7ab4-115">Double</span><span class="sxs-lookup"><span data-stu-id="e7ab4-115">Double</span></span>|<span data-ttu-id="e7ab4-116">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="e7ab4-117">locations</span><span class="sxs-lookup"><span data-stu-id="e7ab4-117">locations</span></span>|<span data-ttu-id="e7ab4-118">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="e7ab4-118">[location](location.md) collection</span></span>|<span data-ttu-id="e7ab4-119">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="e7ab4-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="e7ab4-120">meetingTimeSlot</span></span>|[<span data-ttu-id="e7ab4-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="e7ab4-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="e7ab4-122">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="e7ab4-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="e7ab4-123">organizerAvailability</span></span>|<span data-ttu-id="e7ab4-124">String</span><span class="sxs-lookup"><span data-stu-id="e7ab4-124">String</span></span>| <span data-ttu-id="e7ab4-p101">Доступность организатора собрания для этого варианта собрания. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="e7ab4-127">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="e7ab4-127">suggestionHint</span></span>|<span data-ttu-id="e7ab4-128">String</span><span class="sxs-lookup"><span data-stu-id="e7ab4-128">String</span></span>|<span data-ttu-id="e7ab4-129">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="e7ab4-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
