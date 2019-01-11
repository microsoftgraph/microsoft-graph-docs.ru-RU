---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: 6e3cc56f1495eae60bb84c458caa25c79557e033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832909"
---
# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
