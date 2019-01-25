---
title: Тип ресурса licenseAssignmentState
description: 'Свойство **licenseAssignmentStates** удостоверение пользователя — это коллекция **licenseAssignmentState**. Его предоставляет подробные сведения о назначениях лицензии для пользователя. Сведения о включает в себя сведения, например:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515281"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса licenseAssignmentState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **licenseAssignmentStates** удостоверение [пользователя](user.md) — это коллекция **licenseAssignmentState**. Его предоставляет подробные сведения о назначениях лицензии для пользователя. Сведения о включает в себя сведения, например:  

 - Какие планы отключены для пользователя
 - Ли назначенных пользователю напрямую или наследуется из группы лицензии
 - Текущее состояние назначения
 - Если состояние назначения ошибки, что такое описание ошибки для ошибки 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedByGroup|string|Идентификатор группы, предназначенного для назначения данной лицензии. Если назначения лицензий назначенных прямым, это поле будет Null. Только для чтения.|
|disabledPlans|Collection(String)|Планы обслуживания, которые отключены в этой назначения. Только для чтения.|
|error|String|Сбой назначения лицензий. Если лицензия назначена успешно, в этом поле будет Null. Только для чтения. Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`. Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|Уникальный идентификатор SKU. Только для чтения.|
|state|String|Указывает текущее состояние данного назначения. Только для чтения. Возможные значения: активный, ActiveWithError, отключено и ошибки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
