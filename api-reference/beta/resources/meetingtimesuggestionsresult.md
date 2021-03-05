---
title: Тип ресурса meetingTimeSuggestionsResult
description: Коллекция предложений о собраниях, если они есть, и причина, по которой их нет.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 87b4a2515ced0baf8518b11d6f5e2042211e3483
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471805"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Тип ресурса meetingTimeSuggestionsResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция предложений о собраниях, если они есть, и причина, по которой их нет.

Ниже представлены возможные причины, по которым метод [findMeetingTimes](../api/user-findmeetingtimes.md) может не возвращать предложения.

|**Значение emptySuggestionsReason**|**Причины**|
|:-----|:-----|
| attendeesUnavailable | Доступность всех участников известна, но для достижения порога доверия к [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) собранию, который по умолчанию составляет 50% для любого периода времени, недостаточно.|
| attendeesUnavailableOrUnknown | Отсутствуют сведения о доступности некоторых или всех участников, из-за чего значение достоверности собрания становится ниже заданного порога (значение по умолчанию — 50 %). Доступность участника может стать неизвестной, если он находится за пределами организации или произошла ошибка при получении сведений о доступности.|
| locationsUnavailable | Свойство **isRequired** **параметра locationConstraint** указывается как true, но в расчетных интервалах времени нет расположения. |
| organisUnavailable | Для параметра **isOrganizerOptional** задано значение false, но организатор недоступен в запрашиваемый период времени. |
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
|emptySuggestionsReason|String|Причина отсутствия предложений в результатах. Возможные значения: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` и `unknown`. Это свойство — пустая строка, если свойство **meetingTimeSuggestions** содержит любые предложения о собрании.|
|meetingTimeSuggestions|Коллекция объектов [meetingTimeSuggestion](meetingtimesuggestion.md)|Массив предложений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


