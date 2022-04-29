---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23a0e22fe44cac84f017446326beea052e3c067c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133799"
---
# <a name="patternedrecurrence-resource-type"></a>Тип ресурса patternedRecurrence

Пространство имен: microsoft.graph

Расписание и диапазон повторения. Этот общий объект используется для определения повторения следующих объектов:
+ [Объекты accessReviewScheduleDefinition](accessreviewscheduledefinition.md) в Azure AD API проверки доступа
+ [объекты](event.md) событий в API календаря
+ [объекты unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) и [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) в PIM;
+ [объекты accessPackageAssignment](accesspackageassignment.md) в Azure AD управления правами.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|pattern|[recurrencePattern](recurrencepattern.md)|Частота события. <br/><br/> Для проверок доступа: <li>Не указывайте это свойство для однофакторной проверки доступа. <li> **Поддерживаются только свойства interval**, **dayOfMonth** и **type** (`weekly`,`absoluteMonthly`) [recurrencePattern](recurrencepattern.md).|
|range|[recurrenceRange](recurrencerange.md)|Продолжительность события.|

## <a name="json-representation"></a>Представление в формате JSON

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

