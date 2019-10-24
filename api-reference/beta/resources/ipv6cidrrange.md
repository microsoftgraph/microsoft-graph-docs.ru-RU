---
title: Тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6-адресов с использованием нотации CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7201a95013551aa9629032bffc808f93156f66a0
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653848"
---
# <a name="ipv6cidrrange-resource-type"></a>Тип ресурса iPv6CidrRange

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет диапазон IPv6-адресов с использованием нотации CIDR.

Наследуется от ресурса [ipRange](../resources/iprange.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Цидраддресс|String|IPv6-адрес в нотации CIDR|

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