---
title: Тип ресурсов timeConstraint
description: Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6822aab3521464842278f80fa323da039506afa9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122931"
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

