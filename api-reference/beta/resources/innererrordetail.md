---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a5b85f17b87343766a4edb00c6d620c185ecaf5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939658"
---
# <a name="innererrordetail-resource-type"></a>Тип ресурса Иннереррордетаил

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                  |
|:---------|:-------|:---------------------------------------------|
| message  | String | Сообщение об ошибке, читаемое человеком. Только для чтения. |
| source   | Строка | Источник ошибки. Только для чтения.          |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
