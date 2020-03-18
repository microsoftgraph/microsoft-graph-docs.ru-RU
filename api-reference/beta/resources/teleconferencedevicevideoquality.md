---
title: Тип ресурса Телеконференцедевицевидеокуалити
description: Представляет данные о качестве видео для видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 33b781a5b32285f30b4be1c5941fa75bf836fac3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763237"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="5b397-103">Тип ресурса Телеконференцедевицевидеокуалити</span><span class="sxs-lookup"><span data-stu-id="5b397-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="5b397-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b397-105">Представляет данные о качестве видео для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="5b397-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="5b397-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b397-106">Properties</span></span>

<span data-ttu-id="5b397-107">Ресурс **телеконференцедевицевидеокуалити** наследует свойства от [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)и включает следующие дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="5b397-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="5b397-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b397-108">Property</span></span>     | <span data-ttu-id="5b397-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b397-109">Type</span></span>        | <span data-ttu-id="5b397-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b397-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b397-111">аверажеинбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="5b397-111">averageInboundBitRate</span></span>|<span data-ttu-id="5b397-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5b397-112">Double</span></span>|<span data-ttu-id="5b397-113">Средняя скорость потока для входящего потока в секунду.</span><span class="sxs-lookup"><span data-stu-id="5b397-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="5b397-114">аверажеинбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="5b397-114">averageInboundFrameRate</span></span>|<span data-ttu-id="5b397-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5b397-115">Double</span></span>|<span data-ttu-id="5b397-116">Средняя частота входящего потока видеокадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="5b397-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="5b397-117">аверажеаутбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="5b397-117">averageOutboundBitRate</span></span>|<span data-ttu-id="5b397-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5b397-118">Double</span></span>|<span data-ttu-id="5b397-119">Средняя скорость передачи данных по исходящему потоку в секунду.</span><span class="sxs-lookup"><span data-stu-id="5b397-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="5b397-120">аверажеаутбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="5b397-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="5b397-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5b397-121">Double</span></span>|<span data-ttu-id="5b397-122">Средняя частота исходящих покадровых кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="5b397-122">The average outbound stream video frame rate per second.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b397-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b397-123">JSON representation</span></span>

<span data-ttu-id="5b397-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b397-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceVideoQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
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
  "description": "teleconferenceDeviceVideoQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
