---
title: Тип ресурса Еррордетаил
description: Описание ошибки неудачного запроса на асинхронное создание схемы подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a2ae4137e619620c6dbab12e86a7ed39d4eef13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499164"
---
# <a name="errordetail-resource-type"></a>Тип ресурса Еррордетаил

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание ошибки неудачного запроса на асинхронное создание [схемы](schema.md) подключения Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство  | Тип                                               | Описание |
|:----------|:---------------------------------------------------|:------------|
| подробности   | Коллекция [иннереррордетаил](innererrordetail.md) | Коллекция внутренних ошибок (при наличии). Только для чтения, допускает значение null. |
| errorCode | String                                             | Код ошибки, связанный с ошибкой (при наличии). Только для чтения, допускает значение null. |
| message   | String                                             | Сообщение об ошибке, читаемое человеком. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
