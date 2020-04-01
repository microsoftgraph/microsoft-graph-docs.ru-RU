---
title: Тип ресурса Телеконференцедевицескриншарингкуалити
description: Представляет данные о качестве устройства для демонстрации видеоконференций с видеоконференциями.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7581aba181ad98a15c0cb28067183dea520dbe31
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082765"
---
# <a name="teleconferencedevicescreensharingquality-resource-type"></a><span data-ttu-id="5078b-103">Тип ресурса Телеконференцедевицескриншарингкуалити</span><span class="sxs-lookup"><span data-stu-id="5078b-103">teleconferenceDeviceScreenSharingQuality resource type</span></span>

<span data-ttu-id="5078b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5078b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5078b-105">Представляет данные о качестве устройства для демонстрации видеоконференций с видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="5078b-105">Represents video teleconferencing device screen-sharing quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="5078b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5078b-106">Properties</span></span>

<span data-ttu-id="5078b-107">**Телеконференцедевицескриншарингкуалити** наследует все свойства из [телеконференцедевицевидеокуалити](teleconferencedevicevideoquality.md).</span><span class="sxs-lookup"><span data-stu-id="5078b-107">The **teleconferenceDeviceScreenSharingQuality** inherits all the properties from [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5078b-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5078b-108">JSON representation</span></span>

<span data-ttu-id="5078b-109">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5078b-109">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceScreenSharingQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceVideoQuality"
}-->

```json
{
  "averageInboundBitRate": 1024,
  "averageInboundFrameRate": 1024,
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
  "averageOutboundBitRate": 1024,
  "averageOutboundFrameRate": 1024,
  "averageOutboundJitter": "String (ISO 8601 duration)",
  "averageOutboundPacketLossRateInPercentage": 10,
  "averageOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "channelIndex": 1,
  "inboundPackets": 1024,
  "localIPAddress": "String",
  "localPort": 2000,
  "maximumInboundJitter": "String (ISO 8601 duration)",
  "maximumInboundPacketLossRateInPercentage": 12,
  "maximumInboundRoundTripDelay": "String (ISO 8601 duration)",
  "maximumOutboundJitter": "String (ISO 8601 duration)",
  "maximumOutboundPacketLossRateInPercentage": 12,
  "maximumOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "mediaDuration": "String (ISO 8601 duration)",
  "networkLinkSpeedInBytes": 1000000,
  "outboundPackets": 1024,
  "remoteIPAddress": "String",
  "remotePort": 3000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceScreenSharingQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
