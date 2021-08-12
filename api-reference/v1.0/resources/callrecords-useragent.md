---
title: тип ресурса userAgent
description: Тип userAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a32c74957d0d0a2c41323c1f76d4e990897d61948892821e2d56154eceec271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189921"
---
# <a name="useragent-resource-type"></a>тип ресурса userAgent

Пространство имен: microsoft.graph.callRecords

Представляет агент пользователя конечной точки в вызове.
Типы [clientUserAgent](callrecords-clientuseragent.md) и [serviceUserAgent](callrecords-serviceuseragent.md)наследуют от этого типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого этой конечной точкой.|
|headerValue|String|Значение заглавной точки пользователя-агента, сообщаемого этой конечной точкой.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
