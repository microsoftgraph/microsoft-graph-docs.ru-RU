---
title: Тип ресурса printMargin
description: Указывает ширину полей, используемую при печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7d6d2e0d1f83cb0da747fb0bb901ba21547612c4
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176668"
---
# <a name="printmargin-complex-type"></a>Сложный тип printMargin

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает ширину полей, используемую при печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|top|Int32|Поле в микронах от верхнего края.|
|Нижней|Int32|Поле в микронах от нижнего края.|
|Правильно|Int32|Поле в микронах от правого края.|
|left|Int32|Поле в микронах от левого края.|

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


