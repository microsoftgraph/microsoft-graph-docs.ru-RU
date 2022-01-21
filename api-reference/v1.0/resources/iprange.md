---
title: Тип ресурса ipRange
description: Базовый класс диапазона IP для представления диапазонов адресов IPV4 и IPV6.
ms.localizationpriority: medium
author: davidspooner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a6f963e471e29c17191e8a5710ecef4828c28b60
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161874"
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

