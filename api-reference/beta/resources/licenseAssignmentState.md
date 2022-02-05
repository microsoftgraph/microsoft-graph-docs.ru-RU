---
title: licenseAssignmentState type
description: 'Свойство **licenseAssignmentStates** сущности пользователя — это коллекция **лицензийAssignmentState**. Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
---

# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **licenseAssignmentStates** сущности пользователя — [](user.md) это коллекция **лицензийAssignmentState**. Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:

- Какие планы отключены для пользователя
- Была ли лицензия назначена пользователю напрямую или унаследована от группы
- Текущее состояние назначения
- Если состояние назначения — ошибка, то какая деталь ошибки для сбоя?


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|string|ID группы, которая назначает эту лицензию. Если назначение является прямо назначенной лицензией, это поле будет Null. Только для чтения.|
|disabledPlans|Collection(String)|Планы служб, отключенные в этом назначении. Только для чтения.|
|error|Строка|Ошибка сбоя назначения лицензии. Если лицензия назначена успешно, это поле будет Null. Только для чтения. Возможные значения , `CountViolation``MutuallyExclusiveViolation`, `DependencyViolation`, , `ProhibitedInUsageLocationViolation`и `UniquenessViolation``Other`. Дополнительные сведения о том, как выявлять и устранять ошибки назначения лицензий, см. [здесь](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния назначения лицензии.|
|skuId|Строка|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указать текущее состояние этого назначения. Только для чтения. Возможные значения: `Active`, `ActiveWithError`, `Disabled` и `Error`.|

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
  "lastUpdatedDateTime": "String (timestamp)",
  "skuId": " String ",
  "state": "String"
}

```
