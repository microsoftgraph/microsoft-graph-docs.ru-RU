---
title: Тип ресурса Интежерранже
description: Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c7c3a14e8b8772a0bc319d8415046f3e10871f52
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896038"
---
# <a name="integerrange-resource-type"></a>Тип ресурса Интежерранже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|minimum|Int64|Инклюзивная Нижняя граница диапазона целых чисел.|
|maximum|Int64|Включающая верхняя граница диапазона целых чисел.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "minimum": 12345,
    "maximum": 12345
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "integerRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->