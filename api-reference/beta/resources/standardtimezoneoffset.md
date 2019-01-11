---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
ms.openlocfilehash: 04808d73a6ac41be8eec2959f5ff1d8c5caa44d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841246"
---
# <a name="standardtimezoneoffset-resource-type"></a>Тип ресурса standardTimeZoneOffset

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.

Например, если для указанного часового пояса заданы следующие свойства:

- **dayOccurrence** — 3
- **dayOfWeek** — "Sunday"
- **month** — 10
- **time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| dayOccurrence | Edm.Int32 | Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время. |
| dayOfWeek | строка | Представляет день недели, в который осуществляется переход с летнего времени на стандартное. |
| month | Edm.Int32 | Представляет месяц, когда осуществляется переход с летнего времени на стандартное. |
| time | Edm.TimeOfDay | Представляет время суток, когда происходит переход с летнего времени на стандартное. |
| year | Edm.Int32 | Указывает периодичность перехода с летнего времени на стандартное (в годах). Например, значение "0" указывает, что переход осуществляется ежегодно.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
