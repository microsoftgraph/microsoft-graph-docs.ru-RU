---
title: тип ресурса teleconferenceDeviceVideoQuality
description: Представляет данные о качестве видеоконференции устройства видео.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 30c9c8f383a5d4b41b5c2355a5b2da910d560282aa4e450fa462313d4cb65b34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231427"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a>тип ресурса teleconferenceDeviceVideoQuality

Пространство имен: microsoft.graph

Представляет данные о качестве видеоконференции устройства видео.

## <a name="properties"></a>Свойства

Ресурс **teleconferenceDeviceVideoQuality** наследует свойства [от teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)и включает следующие дополнительные свойства.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|averageInboundBitRate|Двойное с плавающей точкой|Средняя скорость бита видеопотока входящий поток в секунду.|
|averageInboundFrameRate|Двойное с плавающей точкой|Средняя частота кадров видеопотока в потоке в секунду.|
|averageOutboundBitRate|Двойное с плавающей точкой|Средняя скорость потока исходящие видео в секунду.|
|averageOutboundFrameRate|Двойное с плавающей точкой|Средняя частота кадров видеопотока исходящие потоки в секунду.|

### <a name="derived-types"></a>Производные типы

| Тип                                                 | Описание                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | Данные качества видеоконференции устройства для обмена экранами. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

