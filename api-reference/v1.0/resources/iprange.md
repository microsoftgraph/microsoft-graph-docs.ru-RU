---
title: Тип ресурса ipRange
description: Базовый класс диапазона IP для представления диапазонов адресов IPV4 и IPV6.
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b0bb1aba5e0a8f26e12aa8d8f1e273dd58617f68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089384"
---
# <a name="iprange-resource-type"></a>Тип ресурса ipRange

Пространство имен: microsoft.graph

Абстрактный тип диапазона IP, из которого получены типы ресурсов [iPv4CidrRange](ipv4cidrrange.md) и [iPv6CidrRange](ipv6cidrrange.md) для настройки [объектов ipNamedLocation.](ipnamedlocation.md)

Производный [тип iPv4CidrRange](ipv4cidrrange.md) используется для настройки диапазонов адресов IPv4, а производный [тип iPv6CidrRange](ipv6cidrrange.md) используется для настройки диапазонов адресов IPv6.

## <a name="properties"></a>Свойства

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipRange"
}-->

```json
{
    "@odata.type": "#microsoft.graph.ipRange"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

