---
title: Тип ресурса Телеконференцедевицевидеокуалити
description: Представляет данные о качестве видео для видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bbcc0b99a75a61375bcf68dc20d32c4052d4f885
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43511171"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="d3568-103">Тип ресурса Телеконференцедевицевидеокуалити</span><span class="sxs-lookup"><span data-stu-id="d3568-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="d3568-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3568-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3568-105">Представляет данные о качестве видео для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="d3568-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="d3568-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3568-106">Properties</span></span>

<span data-ttu-id="d3568-107">Ресурс **телеконференцедевицевидеокуалити** наследует свойства от [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)и включает следующие дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="d3568-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="d3568-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3568-108">Property</span></span>     | <span data-ttu-id="d3568-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d3568-109">Type</span></span>        | <span data-ttu-id="d3568-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3568-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3568-111">аверажеинбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="d3568-111">averageInboundBitRate</span></span>|<span data-ttu-id="d3568-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d3568-112">Double</span></span>|<span data-ttu-id="d3568-113">Средняя скорость потока для входящего потока в секунду.</span><span class="sxs-lookup"><span data-stu-id="d3568-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="d3568-114">аверажеинбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="d3568-114">averageInboundFrameRate</span></span>|<span data-ttu-id="d3568-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d3568-115">Double</span></span>|<span data-ttu-id="d3568-116">Средняя частота входящего потока видеокадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="d3568-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="d3568-117">аверажеаутбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="d3568-117">averageOutboundBitRate</span></span>|<span data-ttu-id="d3568-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d3568-118">Double</span></span>|<span data-ttu-id="d3568-119">Средняя скорость передачи данных по исходящему потоку в секунду.</span><span class="sxs-lookup"><span data-stu-id="d3568-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="d3568-120">аверажеаутбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="d3568-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="d3568-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d3568-121">Double</span></span>|<span data-ttu-id="d3568-122">Средняя частота исходящих покадровых кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="d3568-122">The average outbound stream video frame rate per second.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="d3568-123">Производные типы</span><span class="sxs-lookup"><span data-stu-id="d3568-123">Derived types</span></span>

| <span data-ttu-id="d3568-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d3568-124">Type</span></span>                                                 | <span data-ttu-id="d3568-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d3568-125">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="d3568-126">телеконференцедевицескриншарингкуалити</span><span class="sxs-lookup"><span data-stu-id="d3568-126">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="d3568-127">Данные о качестве общего доступа устройства для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="d3568-127">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3568-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3568-128">JSON representation</span></span>

<span data-ttu-id="d3568-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3568-129">The following is a JSON representation of the resource.</span></span>

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
