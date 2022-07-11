---
title: Тип ресурса networkInfo
description: Представляет сведения о сети, используемой в вызове.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fe187e7d900b4851de5a647af5313f08394a1ccc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441533"
---
# <a name="networkinfo-resource-type"></a>Тип ресурса networkInfo

Пространство имен: microsoft.graph.callRecords

Представляет сведения о сети, используемой в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|Двойное с плавающей точкой|Доля звонка, когда конечная точка мультимедиа определяла, что доступная пропускная способность или политика пропускной способности достаточно низкая, чтобы вызвать низкое качество отправляемого звука.|
|basicServiceSetIdentifier|String|Идентификатор базового набора служб беспроводной локальной сети конечной точки мультимедиа, используемой для подключения к сети.|
|connectionType|microsoft.graph.callRecords.networkConnectionType|Тип сети, используемой конечной точкой мультимедиа. Возможные значения: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Двойное с плавающей точкой|Доля звонка, когда конечная точка мультимедиа определяла, что задержка сети достаточно значительная, чтобы повлиять на двунастрочную связь в режиме реального времени.|
|dnsSuffix|String|DNS-суффикс, связанный с сетевым адаптером конечной точки мультимедиа.|
|ipAddress|String|IP-адрес конечной точки мультимедиа.|
|linkSpeed|Int64|Скорость связывания в битах в секунду, сообщаемая сетевым адаптером, используемым конечной точкой мультимедиа.|
|macAddress|String|MAC-адрес сетевого устройства конечной точки мультимедиа.|
|networkTransportProtocol|microsoft.graph.callRecords.networkTransportProtocol|Сетевой протокол, используемый для передачи потока. Возможные значения: `unknown`, `udp`, `tcp`, `unknownFutureValue`.|
|Порт|Int32|Номер сетевого порта, используемый конечной точкой мультимедиа.|
|receivedQualityEventRatio|Двойное с плавающей точкой|Доля звонка, когда конечная точка мультимедиа определяла, что сеть вызывает неудовлетворительное качество полученного звука.|
|dressipAddress|String|IP-адрес конечной точки мультимедиа, отображаемой сервером ретрансляции мультимедиа. Обычно это общедоступный IP-адрес Интернета, связанный с конечной точкой.|
|relayIPAddress|String|IP-адрес сервера ретрансляции мультимедиа, выделенного конечной точкой мультимедиа.|
|relayPort|Int32|Номер сетевого порта, выделенный на сервере ретрансляции мультимедиа конечной точкой мультимедиа.|
|sentQualityEventRatio|Двойное с плавающей точкой|Доля звонка, когда конечная точка мультимедиа определяла, что сеть вызывает неудовлетворительное качество отправляемого звука.|
|Подсети|String|Подсеть, используемая для потока мультимедиа конечной точкой мультимедиа.|
|traceRouteHops|[Коллекция microsoft.graph.callRecords.traceRouteHop](callrecords-traceroutehop.md)|Список прыжков маршрута трассировки сети, собранных для этого потока мультимедиа.\*|
|wifiBand|microsoft.graph.callRecords.wifiBand|Диапазон Wi-Fi, используемый конечной точкой мультимедиа. Возможные значения: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.|
|wifiBatteryCharge|Int32|Предполагаемая оставшаяся заряда батареи в процентах, сообщаемая конечной точкой мультимедиа.|
|wifiChannel|Int32|Канал Wi-Fi, используемый конечной точкой мультимедиа.|
|WifiMicrosoftDriver|String|Имя драйвера Wi-Fi (Майкрософт), используемого конечной точкой мультимедиа. Значение может быть локализовано на основе языка, используемого конечной точкой.|
|WifiMicrosoftDriverVersion|String|Версия драйвера Wi-Fi (Майкрософт), используемого конечной точкой мультимедиа.|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|Тип радио Wi-Fi, используемый конечной точкой мультимедиа. Возможные значения: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|Надежность сигнала Wi-Fi в процентах, сообщаемая конечной точкой мультимедиа.|
|wifiVendorDriver|String|Имя драйвера Wi-Fi, используемого конечной точкой мультимедиа. Значение может быть локализовано на основе языка, используемого конечной точкой.|
|WifiVendorDriverVersion|String|Версия драйвера Wi-Fi, используемого конечной точкой мультимедиа.|

> [!NOTE]
> \*По умолчанию **traceRouteHops** всегда возвращает пустой массив. Обратитесь в службу поддержки Майкрософт, чтобы включить отчеты о данных маршрута трассировки для вашей организации.

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
  "linkSpeed": "Int64",
  "macAddress": "String",
  "networkTransportProtocol": "String",
  "port": "Int32",
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": "Int32",
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "traceRouteHops": [{"@odata.type": "microsoft.graph.callRecords.traceRouteHop"}],
  "wifiBand": "String",
  "wifiBatteryCharge": "Int32",
  "wifiChannel": "Int32",
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": "Int32",
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
