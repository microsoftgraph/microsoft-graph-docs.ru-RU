---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4d05d000b2491fcc9d02b3e39bb012e6e5f023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130517"
---
# <a name="customtimezone-resource-type"></a>Тип ресурса customTimeZone

Пространство имен: microsoft.graph

Представляет часовой пояс c нестандартным переходом на летнее время и обратно.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | Смещение времени часового пояса относительно времени в формате UTC. Это значение представлено в минутах. Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее. |
| name | string | Имя настраиваемого часового пояса. |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
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

