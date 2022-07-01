---
title: Тип ресурса traceRouteHop
description: Представляет прыжки маршрута трассировки сети, собранные для потока мультимедиа.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed69c942e8d459ee9101a28d2243d842512c45d2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436605"
---
# <a name="traceroutehop-resource-type"></a>Тип ресурса traceRouteHop

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет прыжки маршрута трассировки сети, собранные для потока [мультимедиа](callrecords-mediastream.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hopCount|Int32|Число сетевых путей этого прыжка, которое использовало для вычисления времени кругового пути.|
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
