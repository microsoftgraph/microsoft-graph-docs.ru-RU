---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506456"
---
# <a name="governanceschedule-resource-type"></a>Тип ресурса Говернанцесчедуле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. 



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
