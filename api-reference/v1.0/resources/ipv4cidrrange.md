---
title: тип ресурса iPv4CidrRange
description: Представляет диапазон IPv4 с помощью нотации CIDR.
ms.localizationpriority: medium
author: davidspooner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5a5d9114ea93150d6391ecc6b18813b97e99cdfd
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161980"
---
# <a name="ipv4cidrrange-resource-type"></a>тип ресурса iPv4CidrRange

Пространство имен: microsoft.graph

Представляет диапазон IPv4 с помощью нотации бесклассовой маршрутизации между доменами (CIDR).

Наследуется от ресурса [ipRange](../resources/iprange.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|cidrAddress|Строка|Адрес IPv4 в нотации CIDR. Значение null не допускается.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv4CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "@odata.type": "#microsoft.graph.iPv4CidrRange",  
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv4CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
