---
title: Тип ресурса Медиастреам
description: Тип Медиастреам
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c75b49c25f0344fa64d56493523c0828d9794a8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394844"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="53263-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="53263-103">mediaStream resource type</span></span>

<span data-ttu-id="53263-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="53263-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53263-105">Представляет сведения о потоке мультимедиа между двумя конечными точками в вызове.</span><span class="sxs-lookup"><span data-stu-id="53263-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="53263-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53263-106">Properties</span></span>

| <span data-ttu-id="53263-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53263-107">Property</span></span>     | <span data-ttu-id="53263-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53263-108">Type</span></span>        | <span data-ttu-id="53263-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53263-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53263-110">аверажеаудиодеградатион</span><span class="sxs-lookup"><span data-stu-id="53263-110">averageAudioDegradation</span></span>|<span data-ttu-id="53263-111">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-111">Double</span></span>|<span data-ttu-id="53263-112">Средняя сеть среднее снижение качества потока для потока.</span><span class="sxs-lookup"><span data-stu-id="53263-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="53263-113">Показывает степень влияния потери и колебаний сети на качество полученного звука.</span><span class="sxs-lookup"><span data-stu-id="53263-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="53263-114">аверажеаудионетворкжиттер</span><span class="sxs-lookup"><span data-stu-id="53263-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="53263-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-115">Duration</span></span>|<span data-ttu-id="53263-116">Средняя колебание для потока, вычисленное, как указано в [RFC 3550][], обозначено в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-117">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-118">аверажебандвидсестимате</span><span class="sxs-lookup"><span data-stu-id="53263-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="53263-119">Int64</span><span class="sxs-lookup"><span data-stu-id="53263-119">Int64</span></span>|<span data-ttu-id="53263-120">Средняя оценка доступной пропускной способности между двумя конечными точками в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="53263-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="53263-121">аверажежиттер</span><span class="sxs-lookup"><span data-stu-id="53263-121">averageJitter</span></span>|<span data-ttu-id="53263-122">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-122">Duration</span></span>|<span data-ttu-id="53263-123">Средняя колебание для потока, вычисленное, как указано в [RFC 3550][], обозначено в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-124">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-125">аверажепаккетлоссрате</span><span class="sxs-lookup"><span data-stu-id="53263-125">averagePacketLossRate</span></span>|<span data-ttu-id="53263-126">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-126">Double</span></span>|<span data-ttu-id="53263-127">Средняя скорость потери пакетов для потока.</span><span class="sxs-lookup"><span data-stu-id="53263-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="53263-128">аверажератиуфконцеаледсамплес</span><span class="sxs-lookup"><span data-stu-id="53263-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="53263-129">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-129">Double</span></span>|<span data-ttu-id="53263-130">Доля количества звуковых кадров с примерами, созданными с помощью скрытия от потери пакетов, к общему количеству звуковых кадров.</span><span class="sxs-lookup"><span data-stu-id="53263-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="53263-131">аверажерецеиведфрамерате</span><span class="sxs-lookup"><span data-stu-id="53263-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="53263-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-132">Double</span></span>|<span data-ttu-id="53263-133">Среднее число кадров в секунду, принимаемых для всех видеопотоков, вычисленное за период сеанса.</span><span class="sxs-lookup"><span data-stu-id="53263-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="53263-134">аверажераундтриптиме</span><span class="sxs-lookup"><span data-stu-id="53263-134">averageRoundTripTime</span></span>|<span data-ttu-id="53263-135">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-135">Duration</span></span>|<span data-ttu-id="53263-136">Среднее время кругового пути распространения сети, вычисленное согласно [спецификации RFC 3550][], обозначенное в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-137">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-138">аверажевидеофрамелоссперцентаже</span><span class="sxs-lookup"><span data-stu-id="53263-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="53263-139">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-139">Double</span></span>|<span data-ttu-id="53263-140">Средний процент потерянных видеокадров, отображаемых для пользователя.</span><span class="sxs-lookup"><span data-stu-id="53263-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="53263-141">аверажевидеофрамерате</span><span class="sxs-lookup"><span data-stu-id="53263-141">averageVideoFrameRate</span></span>|<span data-ttu-id="53263-142">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-142">Double</span></span>|<span data-ttu-id="53263-143">Среднее число кадров в секунду, принимаемых для видеопотока, вычисленное за период сеанса.</span><span class="sxs-lookup"><span data-stu-id="53263-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="53263-144">аверажевидеопаккетлоссрате</span><span class="sxs-lookup"><span data-stu-id="53263-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="53263-145">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-145">Double</span></span>|<span data-ttu-id="53263-146">Средняя доля потерянных пакетов, как указано в [RFC 3550][], вычисленная за время сеанса.</span><span class="sxs-lookup"><span data-stu-id="53263-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="53263-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="53263-147">endDateTime</span></span>|<span data-ttu-id="53263-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53263-148">DateTimeOffset</span></span>|<span data-ttu-id="53263-149">Время в формате UTC при завершении потока.</span><span class="sxs-lookup"><span data-stu-id="53263-149">UTC time when the stream ended.</span></span> <span data-ttu-id="53263-150">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="53263-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53263-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53263-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="53263-152">ловфрамератератио</span><span class="sxs-lookup"><span data-stu-id="53263-152">lowFrameRateRatio</span></span>|<span data-ttu-id="53263-153">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-153">Double</span></span>|<span data-ttu-id="53263-154">Доля звонка, когда частота кадров составляет менее 7,5 кадров в секунду.</span><span class="sxs-lookup"><span data-stu-id="53263-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="53263-155">ловвидеопроцессингкапабилитиратио</span><span class="sxs-lookup"><span data-stu-id="53263-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="53263-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-156">Double</span></span>|<span data-ttu-id="53263-157">Доля вызова, который работает на клиенте менее чем 70% от ожидаемой возможности обработки видео.</span><span class="sxs-lookup"><span data-stu-id="53263-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="53263-158">максаудионетворкжиттер</span><span class="sxs-lookup"><span data-stu-id="53263-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="53263-159">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-159">Duration</span></span>|<span data-ttu-id="53263-160">Максимальное количество колебаний звуковой сети, вычисленное для каждого из 20-секундных окон во время сеанса, обозначенные в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-161">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-162">максжиттер</span><span class="sxs-lookup"><span data-stu-id="53263-162">maxJitter</span></span>|<span data-ttu-id="53263-163">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-163">Duration</span></span>|<span data-ttu-id="53263-164">Максимальный колебаний для потока, вычисленный как указано в RFC 3550, обозначено в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-165">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-166">макспаккетлоссрате</span><span class="sxs-lookup"><span data-stu-id="53263-166">maxPacketLossRate</span></span>|<span data-ttu-id="53263-167">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-167">Double</span></span>|<span data-ttu-id="53263-168">Максимальная скорость потери пакетов для потока.</span><span class="sxs-lookup"><span data-stu-id="53263-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="53263-169">максратиуфконцеаледсамплес</span><span class="sxs-lookup"><span data-stu-id="53263-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="53263-170">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-170">Double</span></span>|<span data-ttu-id="53263-171">Максимальное соотношение пакетов, скрытые средством для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="53263-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="53263-172">максраундтриптиме</span><span class="sxs-lookup"><span data-stu-id="53263-172">maxRoundTripTime</span></span>|<span data-ttu-id="53263-173">Длительность</span><span class="sxs-lookup"><span data-stu-id="53263-173">Duration</span></span>|<span data-ttu-id="53263-174">Максимальное время приема-передачи по сети, вычисленное в соответствии с [RFC 3550][], обозначено в формате [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="53263-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="53263-175">Например, 1 секунда обозначается `'PT1S'`как значение, где "P" — это обозначение времени, а "— это второй указатель.</span><span class="sxs-lookup"><span data-stu-id="53263-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="53263-176">паккетутилизатион</span><span class="sxs-lookup"><span data-stu-id="53263-176">packetUtilization</span></span>|<span data-ttu-id="53263-177">Int64</span><span class="sxs-lookup"><span data-stu-id="53263-177">Int64</span></span>|<span data-ttu-id="53263-178">Число пакетов для потока.</span><span class="sxs-lookup"><span data-stu-id="53263-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="53263-179">постфорвардерроркорректионпаккетлоссрате</span><span class="sxs-lookup"><span data-stu-id="53263-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="53263-180">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="53263-180">Double</span></span>|<span data-ttu-id="53263-181">Скорость потери пакетов после применения FEC для всех видеопотоков и кодеков.</span><span class="sxs-lookup"><span data-stu-id="53263-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="53263-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="53263-182">startDateTime</span></span>|<span data-ttu-id="53263-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53263-183">DateTimeOffset</span></span>|<span data-ttu-id="53263-184">Время в формате UTC при запуске потока.</span><span class="sxs-lookup"><span data-stu-id="53263-184">UTC time when the stream started.</span></span> <span data-ttu-id="53263-185">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="53263-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53263-186">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53263-186">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="53263-187">стреамдиректион</span><span class="sxs-lookup"><span data-stu-id="53263-187">streamDirection</span></span>|<span data-ttu-id="53263-188">String</span><span class="sxs-lookup"><span data-stu-id="53263-188">String</span></span>|<span data-ttu-id="53263-189">Указывает направление потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="53263-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="53263-190">Возможные значения: `callerToCallee`, `calleeToCaller`.</span><span class="sxs-lookup"><span data-stu-id="53263-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="53263-191">стреамид</span><span class="sxs-lookup"><span data-stu-id="53263-191">streamId</span></span>|<span data-ttu-id="53263-192">String</span><span class="sxs-lookup"><span data-stu-id="53263-192">String</span></span>|<span data-ttu-id="53263-193">Уникальный идентификатор для потока.</span><span class="sxs-lookup"><span data-stu-id="53263-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="53263-194">васмедиабипассед</span><span class="sxs-lookup"><span data-stu-id="53263-194">wasMediaBypassed</span></span>|<span data-ttu-id="53263-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="53263-195">Boolean</span></span>|<span data-ttu-id="53263-196">Имеет значение true, если поток мультимедиа обходит сервер-посредник и выполняет прямую связь между клиентом и PSTN Gateway/УАТС, в противном случае false.</span><span class="sxs-lookup"><span data-stu-id="53263-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="53263-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53263-197">JSON representation</span></span>

<span data-ttu-id="53263-198">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53263-198">The following is a JSON representation of the resource.</span></span>

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