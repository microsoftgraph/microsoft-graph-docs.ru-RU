---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778434"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса Лиценсеассигнментстате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  

- Какие планы отключены для пользователя
- Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.
- Текущее состояние назначения
- Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя? 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Ассигнедбиграуп|string|Идентификатор группы, которая назначает эту лицензию. Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null. Только для чтения.|
|Дисабледпланс|Collection(String)|Планы обслуживания, которые отключены в этом назначении. Только для чтения.|
|error|String|Ошибка при назначении лицензии. Если лицензия назначена успешно, это поле будет иметь значение null. Только для чтения. Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`. Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указывает текущее состояние этого назначения. Только для чтения. Возможные значения: Active, Активевисеррор, Disabled и Error.|

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
