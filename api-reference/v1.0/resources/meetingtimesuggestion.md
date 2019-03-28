---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение о собрании, которое включает такие сведения, как время собрания, вероятность посещения, Индивидуальная '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4c5a4cb4d094e7fd7fe9b0e56227a556c6e5b5d1
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936264"
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
|Организераваилабилити|Фрибусистатус| Доступность организатора собрания для этого варианта собрания. Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`|
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
