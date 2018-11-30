---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
ms.openlocfilehash: 5504971618e6b8f6fdb82b203142e84c23c595f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025422"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Тип ресурса meetingTimeSuggestionsResult

Коллекция предложений (если они есть) или причина их отсутствия.

Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.

|**Значение emptySuggestionsReason**|**Причины**|
|:-----|:-----|
| attendeesUnavailable | Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог [достоверности собрания](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) (значение по умолчанию — 50 %).|
| attendeesUnavailableOrUnknown | Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.|
| locationsUnavailable | Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок. |
| organizerUnavailable | Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени. |
| unknown | Причина отсутствия предложений неизвестна.|

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|emptySuggestionsReason|String|Причина не возвращает все предложения о собраниях. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, или `unknown`. Это свойство соответствует пустая строка, если свойство **meetingTimeSuggestions** включают все предложения о собраниях.|
|meetingTimeSuggestions|Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)|Массив предложений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->