---
title: Тип ресурса Девицехеалс
description: Представляет работоспособность устройства, включая все ошибки.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efd8b1e7722eabcacd05512b0101735d677d9b89
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896119"
---
# <a name="devicehealth-resource-type"></a>Тип ресурса Девицехеалс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет работоспособность устройства, включая все ошибки.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|ластконнектионтиме|DateTimeOffset|Время последнего подключения устройства.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceHealth"
}-->

```json
{
    "lastConnectionTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceHealth resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->