---
title: Тип ресурса licenseAssignmentState
description: Свойство **licenseAssignmentStates** сущности пользователя представляет собой коллекцию объектов **licenseAssignmentState** . Он предоставляет сведения о назначениях лицензий пользователю.
author: jconley76
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 2608cb593908380ea3812ce5a1360a015b757050
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549549"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса licenseAssignmentState

Пространство имен: microsoft.graph


Свойство **licenseAssignmentStates** сущности пользователя представляет [](user.md) собой коллекцию объектов **licenseAssignmentState**. Он предоставляет сведения о назначениях лицензий пользователю. Сведения включают следующие сведения:  

- Какие планы отключены для пользователя
- Была ли лицензия назначена пользователю напрямую или унаследована от группы
- Текущее состояние назначения
- Сведения об ошибке, если состояние назначения — Error 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|string|Идентификатор группы, которая назначает эту лицензию. Если назначение является лицензией, назначаемой напрямую, это поле будет иметь значение NULL. Только для чтения.|
|disabledPlans|Collection(String)|Планы обслуживания, которые отключены в этом назначении. Только для чтения.|
|error|String|Ошибка назначения лицензии. Если лицензия назначена успешно, это поле будет иметь значение NULL. Только для чтения. Возможные значения: , , , , `ProhibitedInUsageLocationViolation`и `UniquenessViolation``Other`. `DependencyViolation``MutuallyExclusiveViolation``CountViolation` Дополнительные сведения о том, как выявлять и устранять ошибки назначения лицензий, см. [здесь](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|lastUpdatedDateTime|DateTimeOffset|Метка времени последнего обновления состояния назначения лицензии.|
|skuId|Строка|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Укажите текущее состояние этого назначения. Только для чтения. Возможные значения: `Active`, `ActiveWithError`, `Disabled` и `Error`.|

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
