---
title: Тип ресурса traceRouteHop
description: Представляет прыжки маршрута трассировки сети, собранные для потока мультимедиа.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 31e64989212bc5666b2010d2319bc55bdce11fb6
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924202"
---
# <a name="traceroutehop-resource-type"></a>Тип ресурса traceRouteHop

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет прыжки маршрута трассировки сети, собранные для потока [мультимедиа](callrecords-mediastream.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hopCount|Int32|Число сетевых путей этого прыжка, которое использовало для вычисления RTT.|
|ipAddress|String|IP-адрес, используемый для этого прыжка в трассировке сети.|
|roundTripTime|Длительность|Время отправки пакета маршрута трассировки от клиента к этому прыжку и обратно клиенту в [формате ISO 8601][] . Например, 1 `PT1S`секунда обозначается как ,где P является указателем длительности, T — указателем времени, а S — вторым.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.traceRouteHop"
}-->

```json
{
  "hopCount": "Int32",
  "ipAddress": "String",
  "roundTripTime": "String (duration)"
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
