---
title: Тип ресурса Девицехеалс
description: Представляет работоспособность устройства, включая все ошибки.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7da256308ee63607d7d2d0e7ba62cb3030db4835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049858"
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

