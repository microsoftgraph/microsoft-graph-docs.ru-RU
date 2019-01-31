---
title: Тип ресурса licenseAssignmentState
description: Свойство **licenseAssignmentStates** удостоверение пользователя — это семейство объектов **licenseAssignmentState** . Его предоставляет подробные сведения о назначениях лицензии для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649455"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса licenseAssignmentState


Свойство **licenseAssignmentStates** удостоверение [пользователя](user.md) — это семейство объектов **licenseAssignmentState** . Его предоставляет подробные сведения о назначениях лицензии для пользователя. Эти сведения включают сведения о таких как:  

 - Какие планы отключены для пользователя
 - Ли назначенных пользователю напрямую или наследуется из группы лицензии
 - Текущее состояние назначения
 - Дополнительные сведения об ошибке, если состояние назначения — ошибка 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|string|Идентификатор группы, предназначенного для назначения данной лицензии. Если назначения лицензий назначенных прямым, это поле будет Null. Только для чтения.|
|disabledPlans|Collection(String)|Планы обслуживания, которые отключены в этой назначения. Только для чтения.|
|error|String|Сбой назначения лицензий. Если лицензия назначена успешно, в этом поле будет Null. Только для чтения. Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`. Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указывает текущее состояние данного назначения. Только для чтения. Возможные значения: активный, ActiveWithError, отключено и ошибки.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
