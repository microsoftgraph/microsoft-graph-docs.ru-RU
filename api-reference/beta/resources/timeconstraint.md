---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: 45469211aa4925834fd9d20da6a9905ac87d221e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577237"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="a6cfe-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="a6cfe-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6cfe-104">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="a6cfe-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6cfe-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6cfe-105">JSON representation</span></span>

<span data-ttu-id="a6cfe-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a6cfe-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="a6cfe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6cfe-107">Properties</span></span>
| <span data-ttu-id="a6cfe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6cfe-108">Property</span></span>     | <span data-ttu-id="a6cfe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a6cfe-109">Type</span></span>   |<span data-ttu-id="a6cfe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6cfe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6cfe-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="a6cfe-111">activityDomain</span></span>|<span data-ttu-id="a6cfe-112">String</span><span class="sxs-lookup"><span data-stu-id="a6cfe-112">String</span></span>|<span data-ttu-id="a6cfe-p101">Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a6cfe-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="a6cfe-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="a6cfe-115">timeslots</span></span>|<span data-ttu-id="a6cfe-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="a6cfe-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="a6cfe-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="a6cfe-117">An array of time periods.</span></span>|

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
