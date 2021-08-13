---
title: тип ресурса networkInfo
description: Тип networkInfo
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d12d9364b33a288aa750b565c7fa60157d020a5a9c00eb5092a71c04178ff237
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121440"
---
# <a name="networkinfo-resource-type"></a>тип ресурса networkInfo

Пространство имен: microsoft.graph.callRecords

Представляет сведения о сети, используемой в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|Двойное с плавающей точкой|Доля вызова, который конечная точка мультимедиа обнаружила доступную полосу пропускания или политику пропускной способности, была достаточно низкой, чтобы вызвать плохое качество отправленного звука.|
|basicServiceSetIdentifier|String|Идентификатор базового набора беспроводных lan-служб конечной точки мультимедиа, используемой для подключения к сети.|
|connectionType|microsoft.graph.callRecords.networkConnectionType|Тип сети, используемой конечной точкой мультимедиа. Возможные значения: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Двойное с плавающей точкой|Доля вызова, который конечная точка мультимедиа обнаружила задержку сети, была достаточно значительной, чтобы повлиять на возможность иметь двуназначную связь в режиме реального времени.|
|dnsSuffix|String|Суффикс DNS, связанный с сетевым адаптером конечной точки мультимедиа.|
|ipAddress|String|IP-адрес конечной точки мультимедиа.|
|linkSpeed|Int64|Скорость соединения в битах в секунду сообщается сетевым адаптером, используемым конечной точкой мультимедиа.|
|macAddress|String|Адрес управления доступом к мультимедиа (MAC) сетевого устройства конечной точки мультимедиа.|
|порт|Int32|Номер сетевого порта, используемый конечной точкой мультимедиа.|
|receivedQualityEventRatio|Двойное с плавающей точкой|Незначительная часть вызова, обнаруженного конечной точкой мультимедиа в сети, приводит к низкому качеству полученного звука.|
|reflexiveIPAddress|String|IP-адрес конечной точки мультимедиа, как видно на сервере ретрансляции мультимедиа. Обычно это общедоступный IP-адрес Интернета, связанный с конечной точкой.|
|relayIPAddress|String|IP-адрес сервера ретрансляции мультимедиа, выделенного конечной точкой мультимедиа.|
|relayPort|Int32|Номер сетевого порта, выделенный на сервере ретрансляции мультимедиа конечной точкой мультимедиа.|
|sentQualityEventRatio|Двойное с плавающей точкой|Незначительная часть вызова, обнаруженного конечной точкой мультимедиа в сети, приводит к плохому качеству отосланного звука.|
|подсеть|String|Подсеть, используемая для потока мультимедиа конечной точкой мультимедиа.|
|wifiBand|microsoft.graph.callRecords.wifiBand|Полоса WiFi, используемая конечной точкой мультимедиа. Возможные значения: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.|
|wifiBatteryCharge|Int32|Предполагаемый оставшийся заряд батареи в процентах, о чем сообщает конечная точка мультимедиа.|
|wifiChannel|Int32|Канал WiFi, используемый конечной точкой мультимедиа.|
|wifiMicrosoftDriver|String|Имя драйвера Microsoft WiFi, используемого конечной точкой мультимедиа. Значение может быть локализовано на основе языка, используемого конечной точкой.|
|wifiMicrosoftDriverVersion|String|Версия драйвера Microsoft WiFi, используемого конечной точкой мультимедиа.|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|Тип радио WiFi, используемого конечной точкой мультимедиа. Возможные значения: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|Сила сигнала WiFi в процентах, сообщаемая конечной точкой мультимедиа.|
|wifiVendorDriver|String|Имя драйвера WiFi, используемого конечной точкой мультимедиа. Значение может быть локализовано на основе языка, используемого конечной точкой.|
|wifiVendorDriverVersion|String|Версия драйвера WiFi, используемого конечной точкой мультимедиа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.networkInfo",
  "baseType": null
}-->

```json
{
  "bandwidthLowEventRatio": "Double",
  "basicServiceSetIdentifier": "String",
  "connectionType": "String",
  "delayEventRatio": "Double",
  "dnsSuffix": "String",
  "ipAddress": "String",
  "linkSpeed": 1024,
  "macAddress": "String",
  "port": 1024,
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "wifiBand": "String",
  "wifiBatteryCharge": 1024,
  "wifiChannel": 1024,
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
