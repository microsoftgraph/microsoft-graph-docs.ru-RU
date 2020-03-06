---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d86d5f07a957abe45b898be08744c7c93853d78e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533157"
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
