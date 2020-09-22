---
title: Тип ресурса Телеконференцедевицевидеокуалити
description: Представляет данные о качестве видео для видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8f892fe059828cd7fd71ec19914b5b5db0b9e3cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086230"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="0ff48-103">Тип ресурса Телеконференцедевицевидеокуалити</span><span class="sxs-lookup"><span data-stu-id="0ff48-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="0ff48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ff48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ff48-105">Представляет данные о качестве видео для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="0ff48-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="0ff48-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ff48-106">Properties</span></span>

<span data-ttu-id="0ff48-107">Ресурс **телеконференцедевицевидеокуалити** наследует свойства от [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)и включает следующие дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="0ff48-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="0ff48-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ff48-108">Property</span></span>     | <span data-ttu-id="0ff48-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ff48-109">Type</span></span>        | <span data-ttu-id="0ff48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ff48-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ff48-111">аверажеинбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="0ff48-111">averageInboundBitRate</span></span>|<span data-ttu-id="0ff48-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0ff48-112">Double</span></span>|<span data-ttu-id="0ff48-113">Средняя скорость потока для входящего потока в секунду.</span><span class="sxs-lookup"><span data-stu-id="0ff48-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="0ff48-114">аверажеинбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="0ff48-114">averageInboundFrameRate</span></span>|<span data-ttu-id="0ff48-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0ff48-115">Double</span></span>|<span data-ttu-id="0ff48-116">Средняя частота входящего потока видеокадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="0ff48-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="0ff48-117">аверажеаутбаундбитрате</span><span class="sxs-lookup"><span data-stu-id="0ff48-117">averageOutboundBitRate</span></span>|<span data-ttu-id="0ff48-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0ff48-118">Double</span></span>|<span data-ttu-id="0ff48-119">Средняя скорость передачи данных по исходящему потоку в секунду.</span><span class="sxs-lookup"><span data-stu-id="0ff48-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="0ff48-120">аверажеаутбаундфрамерате</span><span class="sxs-lookup"><span data-stu-id="0ff48-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="0ff48-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0ff48-121">Double</span></span>|<span data-ttu-id="0ff48-122">Средняя частота исходящих покадровых кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="0ff48-122">The average outbound stream video frame rate per second.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="0ff48-123">Производные типы</span><span class="sxs-lookup"><span data-stu-id="0ff48-123">Derived types</span></span>

| <span data-ttu-id="0ff48-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0ff48-124">Type</span></span>                                                 | <span data-ttu-id="0ff48-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0ff48-125">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="0ff48-126">телеконференцедевицескриншарингкуалити</span><span class="sxs-lookup"><span data-stu-id="0ff48-126">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="0ff48-127">Данные о качестве общего доступа устройства для видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="0ff48-127">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ff48-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ff48-128">JSON representation</span></span>

<span data-ttu-id="0ff48-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ff48-129">The following is a JSON representation of the resource.</span></span>

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

