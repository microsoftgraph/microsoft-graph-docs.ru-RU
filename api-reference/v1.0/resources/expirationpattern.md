---
title: Тип ресурса expirationPattern
description: Шаблон срока действия определяет, когда истекает срок действия запроса или назначения.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a42454acfb8c6dc50077fdd85fc7fcf9fa8086e5
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461333"
---
# <a name="expirationpattern-resource-type"></a>Тип ресурса expirationPattern

Пространство имен: microsoft.graph

В [Azure AD управления правами](entitlementmanagement-overview.md) пользователь, желающий получить назначение пакета доступа, создает запрос на назначение пакета доступа. Этот запрос может включать расписание, в течение которых пользователь должен иметь назначение. Назначение пакета для доступа, которое является результатом такого запроса, также имеет расписание. Поле срока действия [объекта entitlementManagementSchedule](entitlementmanagementschedule.md) указывает, когда должно истечь назначение пакета доступа.

В PIM используйте этот ресурс, чтобы определить, когда истекает срок действия объекта [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) или [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) . Параметры, допустимые для этого объекта, зависят от [параметров Azure AD роли](../api/unifiedrolemanagementpolicy-list-rules.md). Например, если параметры роли Azure AD указывают, что постоянные допустимые назначения не допускаются, `noExpiration` указание свойства типа возвращает ошибку.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|duration|Длительность|Требуемая продолжительность доступа запрашиваемого объекта, представленная в формате ISO 8601 для длительности. Например, PT3H ссылается на три часа.  Если этот параметр указан в запросе, **значение endDateTime** не должно присутствовать, а свойству **type** должно быть задано значение `afterDuration`.|
|endDateTime|DateTimeOffset|Метка времени для сведений о дате и времени в формате ISO 8601 и всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|[expirationPatternType](#expirationpatterntype-values)|Требуемый тип шаблона срока действия запрашиваемого объекта. Допустимые значения: `notSpecified`, `noExpiration`, `afterDateTime`, `afterDuration`. |

### <a name="expirationpatterntype-values"></a>Значения expirationPatternType

| Member | Описание |
|:---------------|:--------|
|notSpecified|Расписание окончания срока действия не указано.|
|noExpiration|Инициатор запроса не хочет, чтобы срок действия доступа истек.|
|afterDateTime|Срок действия доступа истекает после указанной даты и времени.|
|afterDuration|Срок действия доступа истекает по истечении указанного периода, относительно предоставленного доступа. Требуется при **указании свойства duration** .|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expirationPattern"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expirationPattern",
  "endDateTime": "String (timestamp)",
  "duration": "String (duration)",
  "type": "String"
}
```


