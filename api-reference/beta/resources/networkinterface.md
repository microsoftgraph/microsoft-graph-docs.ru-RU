---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f19c2fae729e437ec2d9e91a0c6be5694a85214
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812788"
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

## <a name="json-representation"></a>Представление в формате JSON

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
