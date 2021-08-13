---
title: тип ресурса shiftAvailability
description: Доступность пользователя, который должен быть запланирован для работы, и его шаблон повторения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d1c75c5496df6e8d858be74b8001c57fe16de0b3d44a98d4229e1ad09ab77f8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174880"
---
# <a name="shiftavailability-resource-type"></a>тип ресурса shiftAvailability

Пространство имен: microsoft.graph

Доступность пользователя для переноса и [](shift.md) его шаблон повторения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recurrence|[patternedRecurrence](patternedrecurrence.md)| Указывает шаблон для повторения |
|timeSlots|[коллекция timeRange](timerange.md)|Интервал времени(ы) предпочтительный пользователем.|
|timeZone|String|Указывает часовой пояс для указанного времени. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

