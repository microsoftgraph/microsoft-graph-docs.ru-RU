---
title: Тип ресурса Аттендиаваилабилитидатамодел
description: Тип и занятость участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7436a640b4aaba0a9b71ef62ee91b3fe0d7cee
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057418"
---
# <a name="attendeeavailabilitydatamodel-resource-type"></a>Тип ресурса Аттендиаваилабилитидатамодел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя или ресурс, а также их доступность для собрания.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeDataModel"},
  "availability": "String"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|attendee|[Аттендидатамодел](attendeedatamodel.md)|Представляет сведения о лице или ресурсе, а также о том, является ли участник обязательным или необязательным для собрания.|
|availability|availabilityStatus| Состояние доступности участника. Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailabilityDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailabilitydatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->