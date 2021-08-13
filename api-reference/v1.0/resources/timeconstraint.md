---
title: Тип ресурсов timeConstraint
description: Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7b5ed13c523fca24d9b8fad79f6271d4333177c7d2d0f2eece5354423ba370d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221181"
---
# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

Пространство имен: microsoft.graph

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
|activityDomain|activityDomain|Описание действия (необязательно). Возможные значения: `work` , `personal` , , или `unrestricted` `unknown` .|
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

