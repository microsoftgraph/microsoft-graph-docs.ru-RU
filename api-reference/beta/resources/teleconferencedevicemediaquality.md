---
title: Тип ресурса Телеконференцедевицемедиакуалити
description: Данные о качестве устройства мультимедиа для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6fa0bc09f2f6038dd49c8c804420ce042bd5ec93
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510589"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>Тип ресурса Телеконференцедевицемедиакуалити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о качестве устройства мультимедиа для видеоконференций.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|аверажеинбаунджиттер|Длительность|Средняя колебание сети входящего потока.|
|аверажеинбаундпаккетлоссратеинперцентаже|Двойное с плавающей точкой|Средняя скорость потерь пакетов входящих пакетов в процентах (0-100). Например, 0,01 означает 0,01%.|
|аверажеинбаундраундтрипделай|Длительность|Средняя задержка приема для приема в сети для входящего потока.|
|аверажеаутбаунджиттер|Длительность|Средняя колебание сети исходящих потоков.|
|аверажеаутбаундпаккетлоссратеинперцентаже|Двойное с плавающей точкой|Средняя доля потерь пакетов исходящих пакетов в процентах (0-100). Например, 0,01 означает 0,01%.|
|аверажеаутбаундраундтрипделай|Длительность|Средняя задержка циклического приема в сети для исходящего потока.|
|чаннелиндекс|Int32|Индекс канала носителя. Индексация начинается с 1.  Если сеанс мультимедиа содержит 3 видео модальности, индексы каналов будут иметь значение 1, 2 и 3.|
|инбаундпаккетс|Int64|Общее число входящих пакетов.|
|локалипаддресс|String|локальный IP-адрес для сеанса мультимедиа.|
|локалпорт|Int32|Локальный порт мультимедиа.|
|максимуминбаунджиттер|Длительность|Максимальная колебание сети входящего потока.|
|максимуминбаундпаккетлоссратеинперцентаже|Двойное с плавающей точкой|Максимальная скорость потерь пакетов входящих пакетов в процентах (0-100). Например, 0,01 означает 0,01%.|
|максимуминбаундраундтрипделай|Длительность|Максимальная задержка приема для приема в сети для входящего потока.|
|максимумаутбаунджиттер|Длительность|Максимальная колебание сети исходящих потоков.|
|максимумаутбаундпаккетлоссратеинперцентаже|Двойное с плавающей точкой|Максимальная скорость потерь пакетов исходящих пакетов в процентах (0-100). Например, 0,01 означает 0,01%.|
|максимумаутбаундраундтрипделай|Длительность|Максимальная задержка приема в сети для исходящего потока.|
|медиадуратион|Длительность|Общее время модальности. Если мультимедиа включено и отключено несколько раз, Медиадуратион будет вычислить сумму всех этих периодов.|
|нетворклинкспидинбитес|Int64|Скорость сетевого соединения в байтах|
|аутбаундпаккетс|Int64|Общее число исходящих пакетов.|
|ремотеипаддресс|String|Удаленный IP-адрес для сеанса мультимедиа.|
|ремотепорт|Int32|Удаленный порт мультимедиа.|

### <a name="derived-types"></a>Производные типы

| Тип                                                 | Описание                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | Данные о качестве звука устройства видеоконференций для видеоконференций.                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | Данные о качестве видео о качестве видеоконференций для видеоконференций.                          |
| [телеконференцедевицескриншарингкуалити](teleconferencedevicescreensharingquality.md)    | Данные о качестве общего доступа устройства для видеоконференций для видеоконференций. |

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
