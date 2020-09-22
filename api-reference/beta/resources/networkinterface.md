---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d7b712c50d8cc19951f583cb8c9af7e185dba7ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029164"
---
# <a name="networkinterface-resource-type"></a>Тип ресурса Нетворкинтерфаце

Пространство имен: microsoft.graph

Представляет сетевую карту (NIC), связанную с этим узлом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети * < # > и т. д.).|
|ipV4Address|String|Последний IPv4-адрес, связанный с этим сетевым адаптером.|
|ipV6Address|String|Последний открытый (с нестандартным) IPv6-адрес, связанный с этим сетевым адаптером.|
|localIpV6Address|String|IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим сетевым адаптером.|
|macAddress|String|MAC-адрес сетевого адаптера на этом узле.|

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


