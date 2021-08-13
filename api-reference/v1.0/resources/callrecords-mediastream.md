---
title: Тип ресурса mediaStream
description: Тип mediaStream
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2ffa02db859321c09cf329e6404dcb5d065f5a688b19291548205f15858f39ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252104"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

Пространство имен: microsoft.graph.callRecords

Представляет сведения о потоке мультимедиа между двумя конечными точками в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|averageAudioDegradation|Двойное с плавающей точкой|Средняя оценка оценки среднего сетевого мнения для потока. Представляет, насколько потеря сети и испуг повлияли на качество полученного звука.|
|averageAudioNetworkJitter|Длительность|Среднее испуг для потока, вычисляемого в [RFC 3550,][]обозначаемого в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|averageBandwidthEstimate|Int64|Средняя предполагаемая пропускная способность между двумя конечными точками в битах в секунду.|
|averageJitter|Длительность|Среднее испуг для потока, вычисляемого в [RFC 3550,][]обозначаемого в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|averagePacketLossRate|Двойное с плавающей точкой|Средняя скорость потери пакета для потока.|
|averageRatioOfConcealedSamples|Двойное с плавающей точкой|Отношение количества аудиорамок с образцами, созданными в результате сокрытия потери пакетов, к общему числу аудиорамок.|
|averageReceivedFrameRate|Двойное с плавающей точкой|Средние кадры в секунду, полученные для всех видеопотоков, вычисляемого в течение сеанса.|
|averageRoundTripTime|Длительность|Среднее время кругового пути распространения сети, указанное в [RFC 3550,][]обозначается в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|averageVideoFrameLossPercentage|Двойное с плавающей точкой|Средний процент видеорамок, потерянных при отобралении пользователю.|
|averageVideoFrameRate|Двойное с плавающей точкой|Средние кадры в секунду, полученные для видеопотока, вычисляются в течение сеанса.|
|averageVideoPacketLossRate|Двойное с плавающей точкой|Средняя доля потерянных пакетов, как указано в [RFC 3550,][]вычисляется в течение сеанса.|
|endDateTime|DateTimeOffset|Время UTC, когда поток закончился. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lowFrameRateRatio|Двойное с плавающей точкой|Доля вызовов, где частота кадров не превышает 7,5 кадров в секунду.|
|lowVideoProcessingCapabilityRatio|Двойное с плавающей точкой|Доля вызовов, на которые клиент получает менее 70% ожидаемой возможности обработки видео.|
|maxAudioNetworkJitter|Длительность|Максимальное количество висят в аудиосети, вычисляемой на каждом из 20 секундных окон во время сеанса, обозначаемого в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|maxJitter|Длительность|Максимальное испуг для потока, вычисляемого в RFC 3550, обозначаемого в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|maxPacketLossRate|Двойное с плавающей точкой|Максимальная скорость потери пакета для потока.|
|maxRatioOfConcealedSamples|Двойное с плавающей точкой|Максимальное соотношение пакетов, скрытых целителем.|
|maxRoundTripTime|Длительность|Максимальное время кругового распространения сети, указанное в [формате RFC 3550,][]обозначаемого в [формате ISO 8601.][] Например, 1 секунда обозначается как , где "P" является обозначением продолжительности, "T" — это обозначение времени, а S — `'PT1S'` вторым.|
|packetUtilization|Int64|Количество пакетов для потока.|
|postForwardErrorCorrectionPacketLossRate|Двойное с плавающей точкой|Скорость потери пакетов после того, как FEC была применена, агрегирована во всех видеопотоках и кодеках.|
|startDateTime|DateTimeOffset|Время UTC при запущении потока. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|Указывает направление потока мультимедиа. Возможные значения: `callerToCallee`, `calleeToCaller`.|
|streamId|String|Уникальный идентификатор для потока.|
|wasMediaBypassed|Логическое|True, если поток мультимедиа обошел сервер-посредник и пошел прямо между клиентом и PSTN Gateway/PBX, ложным в противном случае.|


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
  "tocPath&quot;: &quot;"
}-->
