---
title: Тип ресурсов timeConstraint
description: Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d79fc1630522c30abea6ac5ec6f51d0f5a15e437
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472113"
---
# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.


## <a name="json-representation"></a>Представление JSON
Ниже показано представление JSON ресурса.

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

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activityDomain|activityDomain|Описание действия (необязательно). Возможные значения: `work` `personal` , , , или `unrestricted` `unknown` .|
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
  "suppressions": []
}
-->


