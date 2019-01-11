---
title: Тип ресурса licenseAssignmentState
description: 'Свойство **licenseAssignmentStates** удостоверение пользователя — это коллекция **licenseAssignmentState**. Его предоставляет подробные сведения о назначениях лицензии для пользователя. Сведения о включает в себя сведения, например:  '
localization_priority: Normal
ms.openlocfilehash: 51ff878f356902362487eda36d17c1894c33e5f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855631"
---
# <a name="licenseassignmentstate-resource-type"></a>Тип ресурса licenseAssignmentState

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|error|Строка|Сбой назначения лицензий. Если лицензия назначена успешно, в этом поле будет Null. Только для чтения. Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`. Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|Строка|Уникальный идентификатор SKU. Только для чтения.|
|state|Строка|Указывает текущее состояние данного назначения. Только для чтения. Возможные значения: активный, ActiveWithError, отключено и ошибки.|

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
