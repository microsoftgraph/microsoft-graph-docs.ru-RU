---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a547329bc6f82ec76d0efc44d7a9e1ffb7700389
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520333"
---
# <a name="standardtimezoneoffset-resource-type"></a>Тип ресурса standardTimeZoneOffset

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| dayOfWeek | string | Представляет день недели, в который осуществляется переход с летнего времени на стандартное. |
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
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
