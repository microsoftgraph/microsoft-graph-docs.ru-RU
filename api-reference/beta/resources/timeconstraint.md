---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519677"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="f3913-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f3913-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3913-104">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="f3913-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3913-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3913-105">JSON representation</span></span>

<span data-ttu-id="f3913-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3913-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="f3913-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3913-107">Properties</span></span>
| <span data-ttu-id="f3913-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3913-108">Property</span></span>     | <span data-ttu-id="f3913-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3913-109">Type</span></span>   |<span data-ttu-id="f3913-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3913-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3913-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="f3913-111">activityDomain</span></span>|<span data-ttu-id="f3913-112">String</span><span class="sxs-lookup"><span data-stu-id="f3913-112">String</span></span>|<span data-ttu-id="f3913-p101">Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f3913-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="f3913-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="f3913-115">timeslots</span></span>|<span data-ttu-id="f3913-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="f3913-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="f3913-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="f3913-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
