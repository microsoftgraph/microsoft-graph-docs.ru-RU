---
title: licenseAssignmentState type
description: 'Свойство **licenseAssignmentStates** объекта пользователя — это коллекция **лицензийAssignmentState.** Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 06b469cb80e92ca09a8e1bce7a058aed1b3a570d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547080"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **licenseAssignmentStates** объекта [](user.md) пользователя — это коллекция **лицензийAssignmentState.** Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:

- Какие планы отключены для пользователя
- Была ли лицензия назначена пользователю напрямую или унаследована от группы
- Текущее состояние назначения
- Если состояние назначения — ошибка, то какая деталь ошибки для сбоя?


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|Строка|ID группы, которая назначает эту лицензию. Если назначение является прямо назначенной лицензией, это поле будет Null. Только для чтения.|
|disabledPlans|Collection(String)|Планы служб, отключенные в этом назначении. Только для чтения.|
|error|String|Ошибка сбоя назначения лицензии. Если лицензия назначена успешно, это поле будет Null. Только для чтения. Возможные значения: `CountViolation` , , , , , и `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` . Дополнительные сведения о том, как выявлять и устранять ошибки назначения лицензий, см. [здесь.](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)|
|skuId|String|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указать текущее состояние этого назначения. Только для чтения. Возможные значения: Active, ActiveWithError, Disabled и Error.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",
  "skuId": "String ",
  "state": "String"
}

```