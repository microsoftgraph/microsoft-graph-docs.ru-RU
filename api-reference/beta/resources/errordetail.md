---
title: Тип ресурса Еррордетаил
description: Описание ошибки неудачного запроса на асинхронное создание схемы подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d52d2953a9ec282b55b021f653854b6c3b6054eb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938992"
---
# <a name="errordetail-resource-type"></a>Тип ресурса Еррордетаил

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание ошибки неудачного запроса на асинхронное создание [схемы](schema.md) подключения Microsoft Search.

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
