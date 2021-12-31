---
title: тип ресурса expirationPattern
description: Шаблон истечения срока действия в расписании запросов может быть включен в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83ec2f3cafc25787a979103f4edea5e6436b57a9
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650694"
---
# <a name="expirationpattern-resource-type"></a>тип ресурса expirationPattern

Пространство имен: microsoft.graph

В [управлении правами Azure AD](entitlementmanagement-overview.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа. Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.  Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.  Поле истечения срока действия [entitlementManagementSchedule](entitlementmanagementschedule.md) указывает, когда должно истекть назначение пакета доступа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|duration|Длительность|Запрашиваемая продолжительность доступа, представленная в формате ISO 8601 для длительности. Например, PT3H — это три часа.  Если указано в запросе, **endDateTime** не должен присутствовать и свойство **типа** должно быть задано `afterDuration` .|
|endDateTime|DateTimeOffset|Время даты и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|[expirationPatternType](#expirationpatterntype-values)|Желаемый тип шаблона истечения срока действия запрашиваемого запроса. Допустимые значения: `notSpecified`, `noExpiration`, `afterDateTime`, `afterDuration`. |

### <a name="expirationpatterntype-values"></a>значения expirationPatternType

| Member | Описание |
|:---------------|:--------|
|notSpecified|Срок действия не указан.|
|noExpiration|Запросчик не хотел, чтобы срок действия доступа истек.|
|afterDateTime|Срок доступа истекает после указанной даты и времени.|
|afterDuration|Срок доступа истекает после указанной продолжительности, относительно предоставленного доступа. Требуется при **указании** свойства продолжительности.|

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


