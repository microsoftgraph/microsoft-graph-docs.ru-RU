---
title: тип ресурса networkInterface
description: Представляет карточку сетевого интерфейса (NIC), связанную с этим хостом.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 914d7f3484762a9b2994fe1eef06d47f4ac09f75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105792"
---
# <a name="networkinterface-resource-type"></a>тип ресурса networkInterface

Пространство имен: microsoft.graph

Представляет карточку сетевого интерфейса (NIC), связанную с этим хостом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание NIC (например, адаптер Ethernet, беспроводный адаптер локального подключения локальной сети *<#> и т.д.).|
|ipV4Address|String|Последний адрес IPv4, связанный с этим NIC.|
|ipV6Address|String|Последний общедоступный (глобальный) адрес IPv6, связанный с этим NIC.|
|localIpV6Address|String|Последний локальный (локализованный или локальный сайт) адрес IPv6, связанный с этим NIC.|
|macAddress|String|MAC-адрес NIC на этом хосте.|

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


