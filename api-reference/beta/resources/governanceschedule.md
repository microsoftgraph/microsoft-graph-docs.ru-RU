---
title: Тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей. '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643414"
---
# <a name="governanceschedule-resource-type"></a>Тип ресурса governanceSchedule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание для [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей. 



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Время начала назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время окончания назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. *Примечание: Если значение равно `null`, указывает постоянное назначение.*|
|type|String|Тип расписания назначения ролей. Только `Once` поддерживается в данный момент.
|duration|Длительность|Длительность назначения ролей. Это в формате интервал времени.|

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
