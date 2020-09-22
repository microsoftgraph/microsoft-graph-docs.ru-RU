---
title: Тип ресурса Интежерранже
description: Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ee879104878189ddcaf51f65e4e127a61798c811
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986058"
---
# <a name="integerrange-resource-type"></a>Тип ресурса Интежерранже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|start|Int64|Инклюзивная Нижняя граница диапазона целых чисел.|
|end|Int64|Включающая верхняя граница диапазона целых чисел.|

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
    "start": 12345,
    "end": 12345
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

