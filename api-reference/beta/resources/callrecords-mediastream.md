---
title: Тип ресурса mediaStream
description: Тип mediaStream
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 180936a2a3bc36e1f7ccd9fe684439caf4531fd7
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924110"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о потоке мультимедиа между двумя конечными точками в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|audioCodec|microsoft.graph.callRecords.audioCodec|Кодекода, используемого для кодирования звука для передачи по сети. Возможные значения: `unknown`, , `invalid``cn`, , `pcma`, `pcmu`, `amrWide`, `g722``g7221`, `g7221c``g729``muchv2``multiChannelAudio`, `rtAudio8``opus``satin``satinFullband``rtAudio16`, , `silk`, , `silkNarrow`, `silkWide`, `siren`, . `xmsRTA``unknownFutureValue`|
|averageAudioDegradation|Двойное с плавающей точкой|Среднее снижение оценки мнений по сети для потока. Представляет, насколько потеря сети и дрожание повлияли на качество полученного звука.|
|averageAudioNetworkJitter|Длительность|Среднее дрожание потока, вычисленного в [формате RFC 3550][], в формате [ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|averageBandwidthEstimate|Int64|Средняя предполагаемая пропускная способность, доступная между двумя конечными точками в битах в секунду.|
|averageJitter|Длительность|Среднее дрожание потока, вычисленного в [формате RFC 3550][], в формате [ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|averagePacketLossRate|Двойное с плавающей точкой|Средняя скорость потери пакетов для потока.|
|averageRatioOfConcealedSamples|Двойное с плавающей точкой|Отношение числа аудиокадров с образцами, созданными при скрытии потери пакетов, к общему количеству аудиокадров.|
|averageReceivedFrameRate|Двойное с плавающей точкой|Среднее число кадров в секунду, полученных для всех видеопотоков, вычисленных за время сеанса.|
|averageRoundTripTime|Длительность|Среднее время кругового пути распространения сети, вычисляемое в [формате RFC 3550][], в формате [ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|averageVideoFrameLossPercentage|Двойное с плавающей точкой|Средний процент потери видеокадров, отображаемый пользователю.|
|averageVideoFrameRate|Двойное с плавающей точкой|Среднее число кадров в секунду, полученных для видеопотока, вычисляется в течение сеанса.|
|averageVideoPacketLossRate|Двойное с плавающей точкой|Средняя доля потерянных пакетов, как указано в [RFC 3550][], вычисляется за время сеанса.|
|endDateTime|DateTimeOffset|Время окончания потока в формате UTC. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lowFrameRateRatio|Двойное с плавающей точкой|Доля звонка, где частота кадров меньше 7,5 кадров в секунду.|
|lowVideoProcessingCapabilityRatio|Двойное с плавающей точкой|Доля звонка, когда клиент выполняет менее 70 % ожидаемой возможности обработки видео.|
|maxAudioNetworkJitter|Длительность|Максимальное количество дрожания аудиосети, вычисленное в каждом из 20 секунд окон во время сеанса, помеченное в формате [ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|maxJitter|Длительность|Максимальное дрожание для потока, вычисленного в формате RFC 3550, в формате [ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|maxPacketLossRate|Двойное с плавающей точкой|Максимальная скорость потери пакетов для потока.|
|maxRatioOfConcealedSamples|Двойное с плавающей точкой|Максимальное соотношение пакетов, скрытых средством исправитель.|
|maxRoundTripTime|Длительность|Максимальное время кругового пути распространения сети, вычисленное в [формате RFC 3550][], указанное в [формате ISO 8601][] . Например, 1 `'PT1S'`секунда обозначается как "P" — это указатель длительности, "T" — указатель времени, а "S" — второй.|
|packetUtilization|Int64|Количество пакетов для потока.|
|postForwardErrorCorrectionPacketLossRate|Двойное с плавающей точкой|Скорость потери пакетов после применения FEC агрегирована по всем видеопотокам и кодекам.|
|startDateTime|DateTimeOffset|Время начала потока в формате UTC. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|Указывает направление потока мультимедиа. Возможные значения: `callerToCallee`, `calleeToCaller`.|
|streamId|Строка|Уникальный идентификатор потока.|
|videoCodec|microsoft.graph.callRecords.videoCodec|Кодекода, используемого для кодирования видео для передачи по сети. Возможные значения: `unknown`, `invalid`, `av1`, `h263`, `h264`, `h264s`, `h264uc`, `h265`, `rtvc1`, `rtVideo`, `xrtvc1`, `unknownFutureValue`.|
|wasMediaBypassed|Boolean|Значение true, если поток мультимедиа обходит сервер-посредник и проходит непосредственно между клиентом и шлюзом ТСОП или УАТС; в противном случае — значение false.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.mediaStream",
  "baseType": null
}-->

```json
{
  "audioCodec": "String",
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
  "videoCodec": "String",
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
  "tocPath&quot;: &quot;"
}-->

