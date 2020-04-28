---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c1dd87e6af015423441b75ada256456e748e3805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495930"
---
# <a name="innererrordetail-resource-type"></a>Тип ресурса Иннереррордетаил

Пространство имен: microsoft.graph

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
