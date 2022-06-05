---
title: Тип ресурса genericError
description: Ошибка общего назначения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: non-product-specific
author: abheek-das
ms.openlocfilehash: 24e54a0efb033347f9bf7479dc9592f97a5fc9e6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899794"
---
# <a name="genericerror-resource-type"></a>Тип ресурса genericError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ошибка общего назначения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| message | String | Сообщение об ошибке. |
| code | Строка | Код ошибки. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```


