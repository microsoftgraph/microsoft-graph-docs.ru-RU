---
title: Тип ресурса mediaStream
description: Тип mediaStream
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 69555033ddacc9244c910b5094449ca60d1a9633
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720258"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="aa4ee-103">Тип ресурса mediaStream</span><span class="sxs-lookup"><span data-stu-id="aa4ee-103">mediaStream resource type</span></span>

<span data-ttu-id="aa4ee-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="aa4ee-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa4ee-105">Представляет сведения о потоке мультимедиа между двумя конечными точками в вызове.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="aa4ee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa4ee-106">Properties</span></span>

| <span data-ttu-id="aa4ee-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa4ee-107">Property</span></span>     | <span data-ttu-id="aa4ee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa4ee-108">Type</span></span>        | <span data-ttu-id="aa4ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4ee-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa4ee-110">averageAudioDegradation</span><span class="sxs-lookup"><span data-stu-id="aa4ee-110">averageAudioDegradation</span></span>|<span data-ttu-id="aa4ee-111">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-111">Double</span></span>|<span data-ttu-id="aa4ee-112">Средняя оценка оценки среднего сетевого мнения для потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="aa4ee-113">Представляет, насколько потеря сети и испуг повлияли на качество полученного звука.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="aa4ee-114">averageAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="aa4ee-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="aa4ee-115">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-115">Duration</span></span>|<span data-ttu-id="aa4ee-116">Среднее испуг для потока, вычисляемого в [RFC 3550,][]обозначаемого в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-117">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-118">averageBandwidthEstimate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="aa4ee-119">Int64</span><span class="sxs-lookup"><span data-stu-id="aa4ee-119">Int64</span></span>|<span data-ttu-id="aa4ee-120">Средняя предполагаемая пропускная способность между двумя конечными точками в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="aa4ee-121">averageJitter</span><span class="sxs-lookup"><span data-stu-id="aa4ee-121">averageJitter</span></span>|<span data-ttu-id="aa4ee-122">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-122">Duration</span></span>|<span data-ttu-id="aa4ee-123">Среднее испуг для потока, вычисляемого в [RFC 3550,][]обозначаемого в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-124">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-125">averagePacketLossRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-125">averagePacketLossRate</span></span>|<span data-ttu-id="aa4ee-126">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-126">Double</span></span>|<span data-ttu-id="aa4ee-127">Средняя скорость потери пакета для потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="aa4ee-128">averageRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="aa4ee-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="aa4ee-129">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-129">Double</span></span>|<span data-ttu-id="aa4ee-130">Отношение количества аудиорамок с образцами, созданными в результате сокрытия потери пакетов, к общему числу аудиорамок.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="aa4ee-131">averageReceivedFrameRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="aa4ee-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-132">Double</span></span>|<span data-ttu-id="aa4ee-133">Средние кадры в секунду, полученные для всех видеопотоков, вычисляемого в течение сеанса.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="aa4ee-134">averageRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="aa4ee-134">averageRoundTripTime</span></span>|<span data-ttu-id="aa4ee-135">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-135">Duration</span></span>|<span data-ttu-id="aa4ee-136">Среднее время кругового пути распространения сети, указанное в [RFC 3550,][]обозначается в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-137">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-138">averageVideoFrameLossPercentage</span><span class="sxs-lookup"><span data-stu-id="aa4ee-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="aa4ee-139">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-139">Double</span></span>|<span data-ttu-id="aa4ee-140">Средний процент видеорамок, потерянных при отобралении пользователю.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="aa4ee-141">averageVideoFrameRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-141">averageVideoFrameRate</span></span>|<span data-ttu-id="aa4ee-142">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-142">Double</span></span>|<span data-ttu-id="aa4ee-143">Средние кадры в секунду, полученные для видеопотока, вычисляются в течение сеанса.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="aa4ee-144">averageVideoPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="aa4ee-145">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-145">Double</span></span>|<span data-ttu-id="aa4ee-146">Средняя доля потерянных пакетов, как указано в [RFC 3550,][]вычисляется в течение сеанса.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="aa4ee-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="aa4ee-147">endDateTime</span></span>|<span data-ttu-id="aa4ee-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa4ee-148">DateTimeOffset</span></span>|<span data-ttu-id="aa4ee-149">Время UTC, когда поток закончился.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-149">UTC time when the stream ended.</span></span> <span data-ttu-id="aa4ee-150">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa4ee-151">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="aa4ee-152">lowFrameRateRatio</span><span class="sxs-lookup"><span data-stu-id="aa4ee-152">lowFrameRateRatio</span></span>|<span data-ttu-id="aa4ee-153">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-153">Double</span></span>|<span data-ttu-id="aa4ee-154">Доля вызовов, где частота кадров не превышает 7,5 кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="aa4ee-155">lowVideoProcessingCapabilityRatio</span><span class="sxs-lookup"><span data-stu-id="aa4ee-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="aa4ee-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-156">Double</span></span>|<span data-ttu-id="aa4ee-157">Доля вызовов, на которые клиент получает менее 70% ожидаемой возможности обработки видео.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="aa4ee-158">maxAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="aa4ee-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="aa4ee-159">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-159">Duration</span></span>|<span data-ttu-id="aa4ee-160">Максимальное количество висят в аудиосети, вычисляемой на каждом из 20 секундных окон во время сеанса, обозначаемого в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-161">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-162">maxJitter</span><span class="sxs-lookup"><span data-stu-id="aa4ee-162">maxJitter</span></span>|<span data-ttu-id="aa4ee-163">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-163">Duration</span></span>|<span data-ttu-id="aa4ee-164">Максимальное испуг для потока, вычисляемого в RFC 3550, обозначаемого в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-165">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-166">maxPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-166">maxPacketLossRate</span></span>|<span data-ttu-id="aa4ee-167">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-167">Double</span></span>|<span data-ttu-id="aa4ee-168">Максимальная скорость потери пакета для потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="aa4ee-169">maxRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="aa4ee-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="aa4ee-170">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-170">Double</span></span>|<span data-ttu-id="aa4ee-171">Максимальное соотношение пакетов, скрытых целителем.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="aa4ee-172">maxRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="aa4ee-172">maxRoundTripTime</span></span>|<span data-ttu-id="aa4ee-173">Duration</span><span class="sxs-lookup"><span data-stu-id="aa4ee-173">Duration</span></span>|<span data-ttu-id="aa4ee-174">Максимальное время кругового распространения сети, указанное в [формате RFC 3550,][]обозначаемого в [формате ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="aa4ee-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="aa4ee-175">Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="aa4ee-176">packetUtilization</span><span class="sxs-lookup"><span data-stu-id="aa4ee-176">packetUtilization</span></span>|<span data-ttu-id="aa4ee-177">Int64</span><span class="sxs-lookup"><span data-stu-id="aa4ee-177">Int64</span></span>|<span data-ttu-id="aa4ee-178">Количество пакетов для потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="aa4ee-179">postForwardErrorCorrectionPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="aa4ee-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="aa4ee-180">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="aa4ee-180">Double</span></span>|<span data-ttu-id="aa4ee-181">Скорость потери пакетов после того, как FEC была применена, агрегирована во всех видеопотоках и кодеках.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="aa4ee-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aa4ee-182">startDateTime</span></span>|<span data-ttu-id="aa4ee-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa4ee-183">DateTimeOffset</span></span>|<span data-ttu-id="aa4ee-184">Время UTC при запущении потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-184">UTC time when the stream started.</span></span> <span data-ttu-id="aa4ee-185">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa4ee-186">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-186">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="aa4ee-187">streamDirection</span><span class="sxs-lookup"><span data-stu-id="aa4ee-187">streamDirection</span></span>|<span data-ttu-id="aa4ee-188">microsoft.graph.callRecords.mediaStreamDirection</span><span class="sxs-lookup"><span data-stu-id="aa4ee-188">microsoft.graph.callRecords.mediaStreamDirection</span></span>|<span data-ttu-id="aa4ee-189">Указывает направление потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="aa4ee-190">Возможные значения: `callerToCallee`, `calleeToCaller`.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="aa4ee-191">streamId</span><span class="sxs-lookup"><span data-stu-id="aa4ee-191">streamId</span></span>|<span data-ttu-id="aa4ee-192">String</span><span class="sxs-lookup"><span data-stu-id="aa4ee-192">String</span></span>|<span data-ttu-id="aa4ee-193">Уникальный идентификатор для потока.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="aa4ee-194">wasMediaBypassed</span><span class="sxs-lookup"><span data-stu-id="aa4ee-194">wasMediaBypassed</span></span>|<span data-ttu-id="aa4ee-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa4ee-195">Boolean</span></span>|<span data-ttu-id="aa4ee-196">True, если поток мультимедиа обошел сервер-посредник и пошел прямо между клиентом и PSTN Gateway/PBX, ложным в противном случае.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="aa4ee-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa4ee-197">JSON representation</span></span>

<span data-ttu-id="aa4ee-198">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa4ee-198">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.mediaStream",
  "baseType": null
}-->

```json
{
  "averageAudioDegradation": "Double",
  "averageAudioNetworkJitter": "String (duration)",
  "averageBandwidthEstimate": 1024,
  "averageJitter": "String (duration)",
  "averagePacketLossRate": "Double",
  "averageRatioOfConcealedSamples": "Double",
  "averageReceivedFrameRate": "Double",
  "averageRoundTripTime": "String (duration)",
  "averageVideoFrameLossPercentage": "Double",
  "averageVideoFrameRate": "Double",
  "averageVideoPacketLossRate": "Double",
  "endDateTime": "String (timestamp)",
  "lowFrameRateRatio": "Double",
  "lowVideoProcessingCapabilityRatio": "Double",
  "maxAudioNetworkJitter": "String (duration)",
  "maxJitter": "String (duration)",
  "maxPacketLossRate": "Double",
  "maxRatioOfConcealedSamples": "Double",
  "maxRoundTripTime": "String (duration)",
  "packetUtilization": 1024,
  "postForwardErrorCorrectionPacketLossRate": "Double",
  "startDateTime": "String (timestamp)",
  "streamDirection": "String",
  "streamId": "String",
  "wasMediaBypassed": true
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
[RFC 3550]: https://tools.ietf.org/html/rfc3550

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

