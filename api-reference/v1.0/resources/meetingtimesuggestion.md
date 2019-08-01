---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение о собрании, которое включает такие сведения, как время собрания, вероятность посещения, Индивидуальная '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 723468d14ebd089d8ed5b020f56e0c70c426ed9b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036206"
---
# <a name="meetingtimesuggestion-resource-type"></a>Тип ресурсов meetingTimeSuggestion

Вариант собрания с такими сведениями, как информация о времени собрания, вероятности участия, занятости отдельных участников, а также доступных расположениях для проведения собрания.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|attendeeAvailability|Коллекция [attendeeAvailability](attendeeavailability.md)|Массив, показывающий состояние занятости каждого участника для этого варианта собрания.|
|confidence|Double|Процент вероятности того, что все участники будут присутствовать на собрании.|
|locations|Коллекция [location](location.md)|Массив, в котором указано имя и географические данные каждого расположения для проведения этого варианта собрания.|
|Митингтимеслот|[timeSlot](timeslot.md)|Период времени, предложенный для собрания.|
|порядке|Int32|Порядок предложений по времени собраний, отсортированных по их вычисленному значению, от высокого до невысокой, затем по чронологи при наличии предложений с одинаковым уровнем достоверности. |
|Организераваилабилити|freeBusyStatus| Доступность организатора собрания для этого варианта собрания. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|Suggestionreason объяснение|String|Обоснование предложенного времени для проведения собрания.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
