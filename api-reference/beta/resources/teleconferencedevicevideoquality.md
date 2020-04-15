---
title: Тип ресурса Телеконференцедевицевидеокуалити
description: Представляет данные о качестве видео для видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ba68e9b6566cde9ede255d2f3a196558621aad7
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510989"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="7d8c3-103">Тип ресурса Телеконференцедевицевидеокуалити</span><span class="sxs-lookup"><span data-stu-id="7d8c3-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="7d8c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d8c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d8c3-105">Представляет данные о качестве видео для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="7d8c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d8c3-106">Properties</span></span>

<span data-ttu-id="7d8c3-107">Ресурс **телеконференцедевицевидеокуалити** наследует свойства от [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)и включает следующие дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="7d8c3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d8c3-108">Property</span></span>     | <span data-ttu-id="7d8c3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7d8c3-109">Type</span></span>        | <span data-ttu-id="7d8c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7d8c3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d8c3-111">аверажеинбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="7d8c3-111">averageInboundBitRate</span></span>|<span data-ttu-id="7d8c3-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7d8c3-112">Double</span></span>|<span data-ttu-id="7d8c3-113">Средняя скорость потока для входящего потока в секунду.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="7d8c3-114">аверажеинбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="7d8c3-114">averageInboundFrameRate</span></span>|<span data-ttu-id="7d8c3-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7d8c3-115">Double</span></span>|<span data-ttu-id="7d8c3-116">Средняя частота входящего потока видеокадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="7d8c3-117">аверажеаутбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="7d8c3-117">averageOutboundBitRate</span></span>|<span data-ttu-id="7d8c3-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7d8c3-118">Double</span></span>|<span data-ttu-id="7d8c3-119">Средняя скорость передачи данных по исходящему потоку в секунду.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="7d8c3-120">аверажеаутбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="7d8c3-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="7d8c3-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7d8c3-121">Double</span></span>|<span data-ttu-id="7d8c3-122">Средняя частота исходящих покадровых кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-122">The average outbound stream video frame rate per second.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="7d8c3-123">Производные типы</span><span class="sxs-lookup"><span data-stu-id="7d8c3-123">Derived types</span></span>

| <span data-ttu-id="7d8c3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7d8c3-124">Type</span></span>                                                 | <span data-ttu-id="7d8c3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7d8c3-125">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="7d8c3-126">телеконференцедевицескриншарингкуалити</span><span class="sxs-lookup"><span data-stu-id="7d8c3-126">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="7d8c3-127">Данные о качестве общего доступа устройства для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-127">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d8c3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d8c3-128">JSON representation</span></span>

<span data-ttu-id="7d8c3-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d8c3-129">The following is a JSON representation of the resource.</span></span>

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
