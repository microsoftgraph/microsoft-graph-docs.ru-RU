---
title: licenseAssignmentState type
description: Свойство **licenseAssignmentStates** объекта пользователя — это коллекция объектов **licenseAssignmentState.** Он предоставляет сведения о назначениях лицензий пользователю.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 40dc8e13240cbeb1fe21bbaabcab38247cee25d2
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493195"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState type

Пространство имен: microsoft.graph


Свойство **licenseAssignmentStates** объекта [](user.md) пользователя — это коллекция объектов **licenseAssignmentState.** Он предоставляет сведения о назначениях лицензий пользователю. Сведения включают такие сведения, как:  

- Какие планы отключены для пользователя
- Была ли лицензия назначена пользователю напрямую или унаследована от группы
- Текущее состояние назначения
- Сведения об ошибках, если состояние назначения — ошибка 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|строка|ID группы, которая назначает эту лицензию. Если назначение является прямо назначенной лицензией, это поле будет Null. Только для чтения.|
|disabledPlans|Collection(String)|Планы служб, отключенные в этом назначении. Только для чтения.|
|error|String|Ошибка сбоя назначения лицензии. Если лицензия назначена успешно, это поле будет Null. Только для чтения. Возможные значения: `CountViolation` , , , , , и `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` . Дополнительные сведения о том, как выявлять и устранять ошибки назначения лицензий, см. [здесь.](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния назначения лицензии.|
|skuId|String|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указать текущее состояние этого назначения. Только для чтения. Возможные значения: Active, ActiveWithError, Disabled и Error.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "lastUpdatedDateTime": "String (timestamp)",
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
