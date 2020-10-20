---
title: Тип ресурса userAgent
description: Тип userAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 55db3bcfc00c54cb51f552624a9e2c51fcce5a7b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601456"
---
# <a name="useragent-resource-type"></a>Тип ресурса userAgent

Пространство имен: microsoft.graph.callRecords

Представляет агента пользователя конечной точки в вызове.
Типы [клиентусеражент](callrecords-clientuseragent.md) и [сервицеусеражент](callrecords-serviceuseragent.md)) наследуются от этого типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого конечной точкой.|
|headerValue|String|Значение заголовка User — Agent, указанное конечной точкой.|

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
