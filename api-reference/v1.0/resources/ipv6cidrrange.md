---
title: тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6 с помощью нотации CIDR.
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a8afeeed483b3610c5c1dde1afee5f4a24317ff4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760864"
---
# <a name="ipv6cidrrange-resource-type"></a>тип ресурса iPv6CidrRange

Пространство имен: microsoft.graph

Представляет диапазон IPv6 с помощью нотации CIDR.

Наследуется от ресурса [ipRange](../resources/iprange.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|cidrAddress|String|Адрес IPv6 в нотации CIDR|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv6CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv6CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
