---
title: Тип ресурса Финдмитингтиместимеконстраинтс
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057422"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a><span data-ttu-id="fb9a7-103">Тип ресурса Финдмитингтиместимеконстраинтс</span><span class="sxs-lookup"><span data-stu-id="fb9a7-103">findMeetingTimesTimeConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb9a7-104">Ограничения времени собраний на характер активности и определенные диапазоны времени. |</span><span class="sxs-lookup"><span data-stu-id="fb9a7-104">Restricts meeting time suggestions to the nature of activity and certain ranges of time.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb9a7-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb9a7-105">JSON representation</span></span>

<span data-ttu-id="fb9a7-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fb9a7-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="fb9a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb9a7-107">Properties</span></span>
| <span data-ttu-id="fb9a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb9a7-108">Property</span></span>     | <span data-ttu-id="fb9a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fb9a7-109">Type</span></span>   |<span data-ttu-id="fb9a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb9a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb9a7-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="fb9a7-111">activityDomain</span></span>|<span data-ttu-id="fb9a7-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="fb9a7-112">activityDomain</span></span>|<span data-ttu-id="fb9a7-p101">Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fb9a7-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="fb9a7-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="fb9a7-115">timeslots</span></span>|<span data-ttu-id="fb9a7-116">Коллекция [сеарчвиндовтимеслот](searchwindowtimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="fb9a7-116">[searchWindowTimeSlot](searchwindowtimeslot.md) collection</span></span>|<span data-ttu-id="fb9a7-117">Массив диапазонов времени для поиска возможных собраний.</span><span class="sxs-lookup"><span data-stu-id="fb9a7-117">An array of time ranges to look into for possible meeting times.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->