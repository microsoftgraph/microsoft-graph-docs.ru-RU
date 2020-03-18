---
title: Тип ресурса Телеконференцедевицеаудиокуалити
description: Данные о качестве звука устройства видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cf2d3be4f0a877f310f1432aede6576fea5897b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763307"
---
# <a name="teleconferencedeviceaudioquality-resource-type"></a><span data-ttu-id="23ef2-103">Тип ресурса Телеконференцедевицеаудиокуалити</span><span class="sxs-lookup"><span data-stu-id="23ef2-103">teleconferenceDeviceAudioQuality resource type</span></span>

<span data-ttu-id="23ef2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ef2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ef2-105">Представляет данные о качестве звука устройства видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="23ef2-105">Represents video teleconferencing device audio quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="23ef2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="23ef2-106">Properties</span></span>

<span data-ttu-id="23ef2-107">**телеконференцедевицеаудиокуалити** наследует все свойства ресурса [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md) .</span><span class="sxs-lookup"><span data-stu-id="23ef2-107">**teleconferenceDeviceAudioQuality** inherits all the properties of the [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23ef2-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23ef2-108">JSON representation</span></span>

<span data-ttu-id="23ef2-109">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23ef2-109">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceAudioQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
}-->

```json
{
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
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
  "description": "teleconferenceDeviceAudioQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
