---
title: тип ресурса userAgent
description: Тип userAgent
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a4154992fd6e187b54a3a794b770e7c53966ce52
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113737"
---
# <a name="useragent-resource-type"></a>тип ресурса userAgent

Пространство имен: microsoft.graph.callRecords

Представляет агент пользователя конечной точки в вызове.
Типы [clientUserAgent](callrecords-clientuseragent.md) и [serviceUserAgent](callrecords-serviceuseragent.md)наследуют от этого типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого этой конечной точкой.|
|headerValue|Строка|Значение заглавной точки пользователя-агента, сообщаемого этой конечной точкой.|

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
