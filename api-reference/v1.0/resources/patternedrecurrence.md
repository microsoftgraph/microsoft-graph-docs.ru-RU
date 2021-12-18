---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f87ffd54073a4e7f414cbcb6c48bf92755cc33cc
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545254"
---
# <a name="patternedrecurrence-resource-type"></a>Тип ресурса patternedRecurrence

Пространство имен: microsoft.graph

Расписание и диапазон повторения. Этот общий объект используется для определения повторения [](event.md)обзоров [доступа,](accessreviewscheduledefinition.md)событий календаря и назначений пакетов доступа [в](accesspackageassignment.md) Azure AD.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|pattern|[recurrencePattern](recurrencepattern.md)|Частота события. <br/><br/> Обзоры доступа: <li>Не укажите это свойство для разового просмотра доступа. <li> **Поддерживаются** только **интервалы, dayOfMonth** и **тип** (, ) свойства `weekly` `absoluteMonthly` [recurrencePattern.](recurrencepattern.md)|
|range|[recurrenceRange](recurrencerange.md)|Продолжительность события.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

