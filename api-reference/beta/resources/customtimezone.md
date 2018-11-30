---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074918"
---
# <a name="customtimezone-resource-type"></a>Тип ресурса customTimeZone

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет часовой пояс c нестандартным переходом на летнее время и обратно.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | Смещение времени часового пояса относительно времени в формате UTC. Это значение представлено в минутах.Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее. |
| name | строка | Имя настраиваемого часового пояса. |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->