---
title: Тип ресурсов meetingTimeSuggestion
description: 'Предложение собрания, которое включает сведения, такие как время собрания, вероятность посещения, индивидуальный '
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d0324b6510b752ffdd21223dc19357ec8392ee24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474017"
---
# <a name="meetingtimesuggestion-resource-type"></a>Тип ресурсов meetingTimeSuggestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "confidence": 1024.0,
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
|meetingTimeSlot|[timeSlot](timeslot.md)|Период времени, предложенный для собрания.|
|порядок|Int32|Порядок предложений по времени собраний, отсортироваться по их вычисляемой уверенности от высокого до низкого, а затем по хронологии, если есть предложения с той же уверенностью. |
|organisAvailability|freeBusyStatus| Доступность организатора собрания для этого варианта собрания. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|suggestionReason|String|Обоснование предложенного времени для проведения собрания.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


