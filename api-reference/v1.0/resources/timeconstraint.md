---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e2ecde664dbdf0335ce84083dfe3c29473c5b1d5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812143"
---
# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

Пространство имен: microsoft.graph

Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.

## <a name="json-representation"></a>Представление в формате JSON

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
|activityDomain|activityDomain|Описание действия (необязательно). Возможные значения: `work` , `personal` , `unrestricted` , или `unknown` .|
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
