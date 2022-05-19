---
title: Тип ресурса licenseAssignmentState
description: 'Свойство **licenseAssignmentStates** сущности пользователя является коллекцией **licenseAssignmentState**. Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jconley76
ms.openlocfilehash: 266e85843aaa7fada2c0e7bd00946ae3e0a6886b
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549570"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса licenseAssignmentState

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **licenseAssignmentStates** сущности пользователя является [](user.md) коллекцией **licenseAssignmentState**. Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:

- Какие планы отключены для пользователя
- Была ли лицензия назначена пользователю напрямую или унаследована от группы
- Текущее состояние назначения
- Если состояние назначения — Error, каковы сведения об ошибке для сбоя?


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
