---
title: Тип ресурса meetingTimeCandidatesResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: ffa8ec3c423da5d94daff4b95cdac52cd511da9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985090"
---
# <a name="meetingtimecandidatesresult-resource-type"></a>Тип ресурса meetingTimeCandidatesResult

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Коллекция предложений (если они есть) или причина их отсутствия.

Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.

|**значение emptySuggestionsHint**|**Причины**|
|:-----|:-----|
| attendeesUnavailable | Имеются сведения о доступности всех участников, но ни для одного периода времени не достигнут порог достоверности собрания (значение по умолчанию — 50 %). Это значение превышено основано на участников состояния занятости для предложенного собрания периода времени со статусом бесплатную участника, соответствующий 100% вероятность присутствия, состояние Нет 50% и % 0 состояние «занят».|
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
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|emptySuggestionsHint|Строка|Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.|
|meetingTimeSlots|[meetingTimeCandidate](meetingtimecandidate.md) коллекции|Массив предложений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
