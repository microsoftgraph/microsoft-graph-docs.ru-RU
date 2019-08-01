---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c5e7461b27168150c21f8fedd5d697e2b8ec5e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036199"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Тип ресурса meetingTimeSuggestionsResult

Коллекция предложений (если они есть) или причина их отсутствия.

Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.

|**Значение emptySuggestionsReason**|**Причины**|
|:-----|:-----|
| Аттендисунаваилабле | Все сведения о доступности участников известны, но недостаточно участников для достижения порогового значения, которое составляет [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) 50% по умолчанию для любого периода времени.|
| Аттендисунаваилаблеорункновн | Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.|
| Локатионсунаваилабле | Свойство **isRequired** параметра [locationConstraint](locationconstraint.md) указано как обязательное, но для рассчитанных периодов времени нет доступных площадок. |
| Организерунаваилабле | Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени. |
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
|Емптисугжестионсреасон|String|Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, или. `unknown` Это свойство представляет собой пустую строку, если в свойстве **митингтимесугжестионс** есть предложения о собраниях.|
|Митингтимесугжестионс|Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)|Массив предложений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
