---
title: Тип ресурса networkInterface
description: Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075513"
---
# <a name="networkinterface-resource-type"></a>Тип ресурса networkInterface

Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|описание|String|Описание сетевого Адаптера (например Ethernet-адаптер, беспроводной Сетевой адаптер подключение по локальной сети * <> # д.).|
|IPv4-адрес|String|Последний IPv4-адрес, связанный с этой сетевого адаптера.|
|IPv6-адрес|String|Последний общедоступных (также называемого глобальные) IPv6 адрес, связанный с этой сетевого адаптера.|
|localIpV6Address|String|Последний локального (локальной связи или локального сайта) IPv6 адрес, связанный с этой сетевого адаптера.|
|macAddress|String|MAC-адрес сетевого Адаптера на этом узле.|

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