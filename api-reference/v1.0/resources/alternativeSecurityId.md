---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d4cdfa609e5cc2daf484bf0f35b863285ee811dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033245"
---
# <a name="alternativesecurityid-resource-type"></a>Тип ресурса alternativeSecurityId

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
| ключа              | EDM. binary | Только для внутреннего использования
