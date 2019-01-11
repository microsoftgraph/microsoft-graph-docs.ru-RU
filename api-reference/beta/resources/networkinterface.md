---
title: Тип ресурса networkInterface
description: Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823305"
---
# <a name="networkinterface-resource-type"></a>Тип ресурса networkInterface

Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|описание|Строка|Описание сетевого Адаптера (например Ethernet-адаптер, беспроводной Сетевой адаптер подключение по локальной сети * <> # д.).|
|IPv4-адрес|Строка|Последний IPv4-адрес, связанный с этой сетевого адаптера.|
|IPv6-адрес|Строка|Последний общедоступных (также называемого глобальные) IPv6 адрес, связанный с этой сетевого адаптера.|
|localIpV6Address|Строка|Последний локального (локальной связи или локального сайта) IPv6 адрес, связанный с этой сетевого адаптера.|
|macAddress|Строка|MAC-адрес сетевого Адаптера на этом узле.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
