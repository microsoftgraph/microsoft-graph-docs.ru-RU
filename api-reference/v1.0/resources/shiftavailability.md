---
title: тип ресурса shiftAvailability
description: Доступность пользователя, который должен быть запланирован для работы, и его шаблон повторения.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e04cbdd14349b4ffc3f01ce22c10948e5fbaff0e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032183"
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

