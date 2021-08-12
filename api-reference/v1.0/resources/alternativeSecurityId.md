---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c2bdac56da724cecce33a43a360ef4cbcdcae6ffea680a35169ce9052d71eeea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229396"
---
# <a name="alternativesecurityid-resource-type"></a>Тип ресурса alternativeSecurityId

Пространство имен: microsoft.graph

Только для внутреннего использования. В будущем этот сложный тип будет обесцениться.

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
| identityProvider | Строка     | Только для внутреннего использования
| ключа              | Edm.Binary | Только для внутреннего использования

