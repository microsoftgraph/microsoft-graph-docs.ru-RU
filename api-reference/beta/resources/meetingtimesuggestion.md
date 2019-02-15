---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение о собрании, которое включает такие сведения, как время собрания, вероятность посещения, Индивидуальная '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057031"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="77273-103">Тип ресурсов meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="77273-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77273-104">Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="77273-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77273-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="77273-105">JSON representation</span></span>

<span data-ttu-id="77273-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="77273-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="77273-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="77273-107">Properties</span></span>
| <span data-ttu-id="77273-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="77273-108">Property</span></span>     | <span data-ttu-id="77273-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77273-109">Type</span></span>   |<span data-ttu-id="77273-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77273-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77273-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="77273-111">attendeeAvailability</span></span>|<span data-ttu-id="77273-112">Коллекция [аттендиаваилабилитидатамодел](attendeeavailabilitydatamodel.md)</span><span class="sxs-lookup"><span data-stu-id="77273-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) collection</span></span>|<span data-ttu-id="77273-113">Массив, показывающий состояние занятости каждого участника для этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="77273-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="77273-114">confidence</span><span class="sxs-lookup"><span data-stu-id="77273-114">confidence</span></span>|<span data-ttu-id="77273-115">Double</span><span class="sxs-lookup"><span data-stu-id="77273-115">Double</span></span>|<span data-ttu-id="77273-116">Процент вероятности того, что все участники будут присутствовать на собрании.</span><span class="sxs-lookup"><span data-stu-id="77273-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="77273-117">locations</span><span class="sxs-lookup"><span data-stu-id="77273-117">locations</span></span>|<span data-ttu-id="77273-118">Коллекция [локатиондатамодел](locationdatamodel.md)</span><span class="sxs-lookup"><span data-stu-id="77273-118">[locationDataModel](locationdatamodel.md) collection</span></span>|<span data-ttu-id="77273-119">Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.</span><span class="sxs-lookup"><span data-stu-id="77273-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="77273-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="77273-120">meetingTimeSlot</span></span>|[<span data-ttu-id="77273-121">Митингтимеслотдатамодел</span><span class="sxs-lookup"><span data-stu-id="77273-121">meetingTimeSlotDataModel</span></span>](meetingtimeslotdatamodel.md)|<span data-ttu-id="77273-122">Период времени, предложенный для собрания.</span><span class="sxs-lookup"><span data-stu-id="77273-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="77273-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="77273-123">organizerAvailability</span></span>|<span data-ttu-id="77273-124">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="77273-124">availabilityStatus</span></span>| <span data-ttu-id="77273-p101">Доступность организатора собрания для этого варианта собрания. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="77273-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="77273-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="77273-127">suggestionReason</span></span>|<span data-ttu-id="77273-128">String</span><span class="sxs-lookup"><span data-stu-id="77273-128">String</span></span>|<span data-ttu-id="77273-129">Обоснование предложенного времени для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="77273-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
