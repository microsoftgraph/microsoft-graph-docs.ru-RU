---
title: Тип ресурса Принтмаргин
description: Задает ширину полей, используемую при печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8f89d2d4daa45d1043e3412852cdaa480223129b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048731"
---
# <a name="printmargin-complex-type"></a>сложный тип Принтмаргин

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает ширину полей, используемую при печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|top|Int32|Маржа в микронах от верхнего края.|
|bottom|Int32|Маржа в микронах от нижнего края.|
|Правильно|Int32|Маржа в микронах от правого края.|
|left|Int32|Маржа в микронах от левого края.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printMargin"
}-->

```json
{
  "top": 123456,
  "bottom": 123456,
  "right": 123456,
  "left": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printMargin resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


