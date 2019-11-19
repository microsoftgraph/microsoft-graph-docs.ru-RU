---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6b3dfb2ec4caf8ae2b8ec9a279a6d001ad3aaae7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703779"
---
# <a name="innererrordetail-resource-type"></a>Тип ресурса Иннереррордетаил

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                  |
|:---------|:-------|:---------------------------------------------|
| message  | String | Сообщение об ошибке, читаемое человеком. Только для чтения. |
| source   | String | Источник ошибки. Только для чтения.          |

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
