---
title: тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса назначения ролей расписание контролирует время выполнения операции назначения ролей, остановку назначения ролей и частое выполнение операции назначения ролей. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 87abccdfac02bea7a3158feb786b39aad23fac3f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694269"
---
# <a name="governanceschedule-resource-type"></a>тип ресурса governanceSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Представляет расписание для [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Для запроса назначения ролей расписание контролирует время выполнения операции назначения ролей, остановку назначения ролей и частое выполнение операции назначения ролей.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|Конечное время назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. *Примечание. Если это `null` значение, оно указывает на постоянное назначение.*|
|type|String|Тип расписания назначения ролей. Только `Once` поддерживается на данный момент.
|duration|Длительность|Продолжительность назначения ролей. Он находится в формате TimeSpan.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


