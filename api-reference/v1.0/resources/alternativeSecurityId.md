---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
author: spunukol
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 151de4ee90d715ffb6619908ea17cd6ba5e52ed4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807852"
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
