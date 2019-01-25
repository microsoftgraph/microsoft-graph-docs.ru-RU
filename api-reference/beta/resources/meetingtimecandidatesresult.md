---
title: Тип ресурса meetingTimeCandidatesResult
description: Коллекция предложений (если они есть) или причина их отсутствия.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: e60c0092ca5724e4019a4c3f75f1239a0e7e9c0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507518"
---
# <a name="meetingtimecandidatesresult-resource-type"></a>Тип ресурса meetingTimeCandidatesResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция предложений (если они есть) или причина их отсутствия.

Ниже представлены возможные причины, по которым метод findMeetingTimes может не возвращать предложения.

|**значение emptySuggestionsHint**|Причины|
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
|emptySuggestionsHint|String|Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`.|
|meetingTimeSlots|[meetingTimeCandidate](meetingtimecandidate.md) коллекции|Массив предложений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidatesresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
