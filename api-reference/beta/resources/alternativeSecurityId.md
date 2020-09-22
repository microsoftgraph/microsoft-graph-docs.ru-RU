---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования. В будущем этот сложный тип будет устаревшим.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: spunukol
ms.openlocfilehash: d08cf247961f4364486f2f9ba5d05508fd900688
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089807"
---
# <a name="alternativesecurityid-resource-type"></a>Тип ресурса alternativeSecurityId

Пространство имен: microsoft.graph

Только для внутреннего использования. В будущем этот сложный тип будет устаревшим.

## <a name="json-representation"></a>Представление JSON

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>Свойства
| Свойство         | Тип       | Описание
|:-----------------|:-----------|:---------------------
| type             | Int32      | Только для внутреннего использования
| identityProvider | string     | Только для внутреннего использования
| ключа              | Edm.Binary | Только для внутреннего использования


