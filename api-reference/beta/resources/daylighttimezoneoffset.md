---
title: Тип ресурса daylightTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 31bd6c1b3e9ec50c2e922ae7868b1d39ea66e4aa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135683"
---
# <a name="daylighttimezoneoffset-resource-type"></a>Тип ресурса daylightTimeZoneOffset

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.

Допустим, для указанного часового пояса заданы следующие свойства:

- **bias** — 300;
- **daylightBias** — -100;
- **dayOccurrence** — 4;
- **dayOfWeek** — "sunday";
- **month** — 5;
- **time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут. Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| daylightBias | Edm.Int32 | Смещение летнего времени относительно времени в формате UTC. Это значение представлено в минутах.  |
| dayOccurrence | Edm.Int32 | Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее. |
| dayOfWeek | строка | Представляет день недели, в который осуществляется переход со стандартного времени на летнее. |
| month | Edm.Int32 | Представляет месяц года, в который осуществляется переход со стандартного времени на летнее. |
| time | Edm.TimeOfDay | Представляет время суток, когда происходит переход со стандартного времени на летнее. |
| year | Edm.Int32 | Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее. Например, значение 0 указывает, что переход осуществляется ежегодно.|


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


