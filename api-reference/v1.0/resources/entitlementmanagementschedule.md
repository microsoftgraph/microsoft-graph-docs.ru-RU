---
title: тип ресурса entitlementManagementSchedule
description: Расписание управления правами может быть включено в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f37a9f58cf6d2ede1393811901c64754d64fd467
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242811"
---
# <a name="entitlementmanagementschedule-complex-type"></a>сложный тип entitlementManagementSchedule

Пространство имен: microsoft.graph

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа. Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.  Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|истечение срока действия|[expirationPattern](../resources/expirationpattern.md)|По истечении срока действия доступа.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Для повторного доступа. Не используется в настоящее время.|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.entitlementManagementSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```


