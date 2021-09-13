---
title: тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6 с помощью нотации CIDR.
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d36d19d3d0d10da58a3223c146be542c9f57878c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062483"
---
# <a name="ipv6cidrrange-resource-type"></a>тип ресурса iPv6CidrRange

Пространство имен: microsoft.graph

Представляет диапазон IPv6 с помощью нотации бесклассовой маршрутизации между доменами (CIDR).

Наследуется от ресурса [ipRange](../resources/iprange.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|cidrAddress|String|Адрес IPv6 в нотации CIDR. Значение null не допускается.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "@odata.type": "#microsoft.graph.iPv6CidrRange", 
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
