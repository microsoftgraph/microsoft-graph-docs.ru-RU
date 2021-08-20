---
title: тип ресурса networkInterface
description: Представляет карточку сетевого интерфейса (NIC), связанную с этим хостом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7ba1efe14cfd4bce099960406ae31392c10529ba862c388e379ef234c786d6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224259"
---
# <a name="networkinterface-resource-type"></a>тип ресурса networkInterface

Пространство имен: microsoft.graph

Представляет карточку сетевого интерфейса (NIC), связанную с этим хостом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|Строка|Описание NIC (например, адаптер Ethernet, беспроводный адаптер локального подключения локальной сети *<#> и т.д.).|
|ipV4Address|Строка|Последний адрес IPv4, связанный с этим NIC.|
|ipV6Address|Строка|Последний общедоступный (глобальный) адрес IPv6, связанный с этим NIC.|
|localIpV6Address|Строка|Последний локальный (локализованный или локальный сайт) адрес IPv6, связанный с этим NIC.|
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


