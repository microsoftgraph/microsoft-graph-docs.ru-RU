---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643568"
---
# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activityDomain|String|Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.|
|timeslots|Коллекция [timeSlot](timeslot.md)|Массив, содержащий значения периодов времени.|

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
