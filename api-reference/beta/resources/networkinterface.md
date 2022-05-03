---
title: Тип ресурса networkInterface
description: Представляет карту сетевого интерфейса (NIC), связанную с этим узлом.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: preetikr
ms.openlocfilehash: 9c2d2b8558730a832d6658ce6ef137d609a13d04
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176807"
---
# <a name="networkinterface-resource-type"></a>Тип ресурса networkInterface

Пространство имен: microsoft.graph

Представляет карту сетевого интерфейса (NIC), связанную с этим узлом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|Строка|Описание сетевого адаптера (например, адаптера Ethernet, подключения к локальной сети беспроводного адаптера локальной сети *<#> и т. д.).|
|ipV4Address|Строка|Последний IPv4-адрес, связанный с этой сетевой картой.|
|ipV6Address|Строка|Последний общедоступный (глобальный) IPv6-адрес, связанный с этой сетевой картой.|
|localIpV6Address|Строка|Последний локальный (локальный или локальный сайт) IPv6-адрес, связанный с этой сетевой картой.|
|macAddress|Строка|MAC-адрес сетевой карты на этом узле.|

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


