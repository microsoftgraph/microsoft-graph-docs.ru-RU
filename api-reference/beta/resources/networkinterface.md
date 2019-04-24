---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457069"
---
# <a name="networkinterface-resource-type"></a>Тип ресурса Нетворкинтерфаце

Представляет сетевую карту (NIC), связанную с этим узлом.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети * _Лт_ # _Гт_ и т. д.).|
|ipV4Address|Строка|Последний IPv4-адрес, связанный с этим СЕТЕВЫМ АДАПТЕРом.|
|ipV6Address|Строка|Последний открытый (с нестандартным) IPv6-адрес, связанный с этим СЕТЕВЫМ АДАПТЕРом.|
|localIpV6Address|Строка|IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим СЕТЕВЫМ АДАПТЕРом.|
|macAddress|Строка|MAC-адрес сетевого адаптера на этом узле.|

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
