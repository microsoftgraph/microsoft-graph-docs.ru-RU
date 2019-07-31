---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36a2b4c73f5f85439a34a42ea2aa23cfe861c4ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006376"
---
# <a name="governanceschedule-resource-type"></a>Тип ресурса Говернанцесчедуле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. 



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время окончания назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. *Note: Если значение задано `null`, оно указывает на постоянное назначение.*|
|type|String|Тип расписания назначения ролей. Поддерживается `Once` только в настоящее время.
|duration|Duration (Длительность)|Продолжительность назначения роли. Он имеет формат TimeSpan.|

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
