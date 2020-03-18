---
title: Тип ресурса Телеконференцедевицемедиакуалити
description: Данные о качестве устройства мультимедиа для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ab703760246fe08145924fd5d21ce4d02a5090b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763311"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a><span data-ttu-id="b73c3-103">Тип ресурса Телеконференцедевицемедиакуалити</span><span class="sxs-lookup"><span data-stu-id="b73c3-103">teleconferenceDeviceMediaQuality resource type</span></span>

<span data-ttu-id="b73c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b73c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b73c3-105">Представляет данные о качестве устройства мультимедиа для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="b73c3-105">Represents video teleconferencing device media quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="b73c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b73c3-106">Properties</span></span>

| <span data-ttu-id="b73c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b73c3-107">Property</span></span>     | <span data-ttu-id="b73c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b73c3-108">Type</span></span>        | <span data-ttu-id="b73c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b73c3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b73c3-110">аверажеинбаунджиттер</span><span class="sxs-lookup"><span data-stu-id="b73c3-110">averageInboundJitter</span></span>|<span data-ttu-id="b73c3-111">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-111">Duration</span></span>|<span data-ttu-id="b73c3-112">Средняя колебание сети входящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-112">The average inbound stream network jitter.</span></span>|
|<span data-ttu-id="b73c3-113">аверажеинбаундпаккетлоссратеинперцентаже</span><span class="sxs-lookup"><span data-stu-id="b73c3-113">averageInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="b73c3-114">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b73c3-114">Double</span></span>|<span data-ttu-id="b73c3-115">Средняя скорость потерь пакетов входящих пакетов в процентах (0-100).</span><span class="sxs-lookup"><span data-stu-id="b73c3-115">The average inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="b73c3-116">Например, 0,01 означает 0,01%.</span><span class="sxs-lookup"><span data-stu-id="b73c3-116">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="b73c3-117">аверажеинбаундраундтрипделай</span><span class="sxs-lookup"><span data-stu-id="b73c3-117">averageInboundRoundTripDelay</span></span>|<span data-ttu-id="b73c3-118">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-118">Duration</span></span>|<span data-ttu-id="b73c3-119">Средняя задержка приема для приема в сети для входящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-119">The average inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="b73c3-120">аверажеаутбаунджиттер</span><span class="sxs-lookup"><span data-stu-id="b73c3-120">averageOutboundJitter</span></span>|<span data-ttu-id="b73c3-121">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-121">Duration</span></span>|<span data-ttu-id="b73c3-122">Средняя колебание сети исходящих потоков.</span><span class="sxs-lookup"><span data-stu-id="b73c3-122">The average outbound stream network jitter.</span></span>|
|<span data-ttu-id="b73c3-123">аверажеаутбаундпаккетлоссратеинперцентаже</span><span class="sxs-lookup"><span data-stu-id="b73c3-123">averageOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="b73c3-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b73c3-124">Double</span></span>|<span data-ttu-id="b73c3-125">Средняя доля потерь пакетов исходящих пакетов в процентах (0-100).</span><span class="sxs-lookup"><span data-stu-id="b73c3-125">The average outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="b73c3-126">Например, 0,01 означает 0,01%.</span><span class="sxs-lookup"><span data-stu-id="b73c3-126">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="b73c3-127">аверажеаутбаундраундтрипделай</span><span class="sxs-lookup"><span data-stu-id="b73c3-127">averageOutboundRoundTripDelay</span></span>|<span data-ttu-id="b73c3-128">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-128">Duration</span></span>|<span data-ttu-id="b73c3-129">Средняя задержка циклического приема в сети для исходящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-129">The average outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="b73c3-130">чаннелиндекс</span><span class="sxs-lookup"><span data-stu-id="b73c3-130">channelIndex</span></span>|<span data-ttu-id="b73c3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b73c3-131">Int32</span></span>|<span data-ttu-id="b73c3-132">Индекс канала носителя.</span><span class="sxs-lookup"><span data-stu-id="b73c3-132">The channel index of media.</span></span> <span data-ttu-id="b73c3-133">Индексация начинается с 1.</span><span class="sxs-lookup"><span data-stu-id="b73c3-133">Indexing begins with 1.</span></span>  <span data-ttu-id="b73c3-134">Если сеанс мультимедиа содержит 3 видео модальности, индексы каналов будут иметь значение 1, 2 и 3.</span><span class="sxs-lookup"><span data-stu-id="b73c3-134">If a media session contains 3 video modalities, channel indexes will be 1, 2, and 3.</span></span>|
|<span data-ttu-id="b73c3-135">инбаундпаккетс</span><span class="sxs-lookup"><span data-stu-id="b73c3-135">inboundPackets</span></span>|<span data-ttu-id="b73c3-136">Int64</span><span class="sxs-lookup"><span data-stu-id="b73c3-136">Int64</span></span>|<span data-ttu-id="b73c3-137">Общее число входящих пакетов.</span><span class="sxs-lookup"><span data-stu-id="b73c3-137">The total number of the inbound packets.</span></span>|
|<span data-ttu-id="b73c3-138">локалипаддресс</span><span class="sxs-lookup"><span data-stu-id="b73c3-138">localIPAddress</span></span>|<span data-ttu-id="b73c3-139">String</span><span class="sxs-lookup"><span data-stu-id="b73c3-139">String</span></span>|<span data-ttu-id="b73c3-140">локальный IP-адрес для сеанса мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b73c3-140">the local IP address for the media session.</span></span>|
|<span data-ttu-id="b73c3-141">локалпорт</span><span class="sxs-lookup"><span data-stu-id="b73c3-141">localPort</span></span>|<span data-ttu-id="b73c3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b73c3-142">Int32</span></span>|<span data-ttu-id="b73c3-143">Локальный порт мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b73c3-143">The local media port.</span></span>|
|<span data-ttu-id="b73c3-144">максимуминбаунджиттер</span><span class="sxs-lookup"><span data-stu-id="b73c3-144">maximumInboundJitter</span></span>|<span data-ttu-id="b73c3-145">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-145">Duration</span></span>|<span data-ttu-id="b73c3-146">Максимальная колебание сети входящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-146">The maximum inbound stream network jitter.</span></span>|
|<span data-ttu-id="b73c3-147">максимуминбаундпаккетлоссратеинперцентаже</span><span class="sxs-lookup"><span data-stu-id="b73c3-147">maximumInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="b73c3-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b73c3-148">Double</span></span>|<span data-ttu-id="b73c3-149">Максимальная скорость потерь пакетов входящих пакетов в процентах (0-100).</span><span class="sxs-lookup"><span data-stu-id="b73c3-149">The maximum inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="b73c3-150">Например, 0,01 означает 0,01%.</span><span class="sxs-lookup"><span data-stu-id="b73c3-150">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="b73c3-151">максимуминбаундраундтрипделай</span><span class="sxs-lookup"><span data-stu-id="b73c3-151">maximumInboundRoundTripDelay</span></span>|<span data-ttu-id="b73c3-152">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-152">Duration</span></span>|<span data-ttu-id="b73c3-153">Максимальная задержка приема для приема в сети для входящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-153">The maximum inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="b73c3-154">максимумаутбаунджиттер</span><span class="sxs-lookup"><span data-stu-id="b73c3-154">maximumOutboundJitter</span></span>|<span data-ttu-id="b73c3-155">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-155">Duration</span></span>|<span data-ttu-id="b73c3-156">Максимальная колебание сети исходящих потоков.</span><span class="sxs-lookup"><span data-stu-id="b73c3-156">The maximum outbound stream network jitter.</span></span>|
|<span data-ttu-id="b73c3-157">максимумаутбаундпаккетлоссратеинперцентаже</span><span class="sxs-lookup"><span data-stu-id="b73c3-157">maximumOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="b73c3-158">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b73c3-158">Double</span></span>|<span data-ttu-id="b73c3-159">Максимальная скорость потерь пакетов исходящих пакетов в процентах (0-100).</span><span class="sxs-lookup"><span data-stu-id="b73c3-159">The maximum outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="b73c3-160">Например, 0,01 означает 0,01%.</span><span class="sxs-lookup"><span data-stu-id="b73c3-160">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="b73c3-161">максимумаутбаундраундтрипделай</span><span class="sxs-lookup"><span data-stu-id="b73c3-161">maximumOutboundRoundTripDelay</span></span>|<span data-ttu-id="b73c3-162">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-162">Duration</span></span>|<span data-ttu-id="b73c3-163">Максимальная задержка приема в сети для исходящего потока.</span><span class="sxs-lookup"><span data-stu-id="b73c3-163">The maximum outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="b73c3-164">медиадуратион</span><span class="sxs-lookup"><span data-stu-id="b73c3-164">mediaDuration</span></span>|<span data-ttu-id="b73c3-165">Длительность</span><span class="sxs-lookup"><span data-stu-id="b73c3-165">Duration</span></span>|<span data-ttu-id="b73c3-166">Общее время модальности.</span><span class="sxs-lookup"><span data-stu-id="b73c3-166">The total modality duration.</span></span> <span data-ttu-id="b73c3-167">Если мультимедиа включено и отключено несколько раз, Медиадуратион будет вычислить сумму всех этих периодов.</span><span class="sxs-lookup"><span data-stu-id="b73c3-167">If the media enabled and disabled multiple times, MediaDuration will the summation of all of the durations.</span></span>|
|<span data-ttu-id="b73c3-168">нетворклинкспидинбитес</span><span class="sxs-lookup"><span data-stu-id="b73c3-168">networkLinkSpeedInBytes</span></span>|<span data-ttu-id="b73c3-169">Int64</span><span class="sxs-lookup"><span data-stu-id="b73c3-169">Int64</span></span>|<span data-ttu-id="b73c3-170">Скорость сетевого соединения в байтах</span><span class="sxs-lookup"><span data-stu-id="b73c3-170">The network link speed in bytes</span></span>|
|<span data-ttu-id="b73c3-171">аутбаундпаккетс</span><span class="sxs-lookup"><span data-stu-id="b73c3-171">outboundPackets</span></span>|<span data-ttu-id="b73c3-172">Int64</span><span class="sxs-lookup"><span data-stu-id="b73c3-172">Int64</span></span>|<span data-ttu-id="b73c3-173">Общее число исходящих пакетов.</span><span class="sxs-lookup"><span data-stu-id="b73c3-173">The total number of the outbound packets.</span></span>|
|<span data-ttu-id="b73c3-174">ремотеипаддресс</span><span class="sxs-lookup"><span data-stu-id="b73c3-174">remoteIPAddress</span></span>|<span data-ttu-id="b73c3-175">String</span><span class="sxs-lookup"><span data-stu-id="b73c3-175">String</span></span>|<span data-ttu-id="b73c3-176">Удаленный IP-адрес для сеанса мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b73c3-176">The remote IP address for the media session.</span></span>|
|<span data-ttu-id="b73c3-177">ремотепорт</span><span class="sxs-lookup"><span data-stu-id="b73c3-177">remotePort</span></span>|<span data-ttu-id="b73c3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b73c3-178">Int32</span></span>|<span data-ttu-id="b73c3-179">Удаленный порт мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b73c3-179">The remote media port.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b73c3-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b73c3-180">JSON representation</span></span>

<span data-ttu-id="b73c3-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b73c3-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality",
  "baseType": null
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
  "description": "teleconferenceDeviceMediaQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
