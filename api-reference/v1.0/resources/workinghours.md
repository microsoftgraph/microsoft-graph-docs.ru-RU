---
title: Тип ресурса workingHours
description: Представляет дни недели и часы работы пользователя в определенном часовом поясе.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 63460f95e419a6e1e39a1c52fbf17d05ef9f5a5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015017"
---
# <a name="workinghours-resource-type"></a>Тип ресурса workingHours

Пространство имен: microsoft.graph

Представляет дни недели и часы работы пользователя в определенном часовом поясе.

Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы. Вы можете [получать](../api/user-get-mailboxsettings.md#example-3) и [задавать](../api/user-update-mailboxsettings.md#example-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxsettings.md). 

Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook. Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете. Для клиента Outlook  
можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.
Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| daysOfWeek | Коллекция dayOfWeek | Дни недели, в которые работает пользователь. |
| startTime | Edm.TimeOfDay | Время дня, в которое пользователь начинает работать. |
| endTime | Edm.TimeOfDay | Время дня, в которое пользователь заканчивает работать. |
| timeZone | [timeZoneBase](timezonebase.md) | Часовой пояс, к которому относится рабочее время. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "String (timeofday)",
  "endTime": "String (timeofday)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->

