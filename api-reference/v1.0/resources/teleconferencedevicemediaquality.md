---
title: тип ресурса teleconferenceDeviceMediaQuality
description: Данные о качестве устройства видеоконференции.
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45ca9d4bdc34077ea19bdcbac866495a198ea5ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128132"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>тип ресурса teleconferenceDeviceMediaQuality

Пространство имен: microsoft.graph

Представляет данные о качестве устройства видеоконференции.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|averageInboundJitter|Длительность|Среднее входящий поток сети испуг.|
|averageInboundPacketLossRateInPercentage|Двойное с плавающей точкой|Средняя скорость потери пакетов входящие потоки в процентах (0-100). Например, 0.01 означает 0.01%.|
|averageInboundRoundTripDelay|Длительность|Средняя задержка входящие потоки сети круглой поездки.|
|averageOutboundJitter|Длительность|Среднее испуг сети исходящие потоки.|
|averageOutboundPacketLossRateInPercentage|Двойное с плавающей точкой|Средняя скорость потери пакетов исходящие потоки в процентах (0-100). Например, 0.01 означает 0.01%.|
|averageOutboundRoundTripDelay|Длительность|Средняя задержка в маршрутной сети исходящие потоки.|
|channelIndex|Int32|Индекс канала мультимедиа. Индексация начинается с 1.  Если сеанс мультимедиа содержит 3 видео модальности, индексы каналов будут 1, 2 и 3.|
|inboundPackets|Int64|Общее число входящие пакеты.|
|localIPAddress|String|локальный IP-адрес сеанса мультимедиа.|
|localPort|Int32|Локальный порт мультимедиа.|
|maximumInboundJitter|Длительность|Максимальный испуг сети входящий поток.|
|maximumInboundPacketLossRateInPercentage|Двойное с плавающей точкой|Максимальная скорость потери пакетов входящий поток в процентах (0-100). Например, 0.01 означает 0.01%.|
|maximumInboundRoundTripDelay|Длительность|Максимальная задержка входящие потоки сети в круглую поездку.|
|maximumOutboundJitter|Длительность|Максимальный испуг сети исходящие потоки.|
|maximumOutboundPacketLossRateInPercentage|Двойное с плавающей точкой|Максимальная скорость потери пакетов исходящие потоки в процентах (0-100). Например, 0.01 означает 0.01%.|
|maximumOutboundRoundTripDelay|Длительность|Максимальная задержка в сети исходящие потоки в округлые поездки.|
|mediaDuration|Длительность|Общая продолжительность модальности. Если мультимедиа включено и отключено несколько раз, mediaDuration будет суммированием всех продолжительности.|
|networkLinkSpeedInBytes|Int64|Скорость сетевых ссылок в bytes|
|outboundPackets|Int64|Общее число исходящие пакеты.|
|remoteIPAddress|Строка|Удаленный IP-адрес сеанса мультимедиа.|
|remotePort|Int32|Удаленный порт мультимедиа.|

### <a name="derived-types"></a>Производные типы

| Тип                                                 | Описание                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | Данные качества звука устройства видеоконференции.                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | Данные качества видеоконференции устройства видео.                          |
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | Данные качества видеоконференции устройства для обмена экранами. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

