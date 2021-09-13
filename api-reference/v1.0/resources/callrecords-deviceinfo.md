---
title: Тип ресурса deviceInfo
description: Тип deviceInfo
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc7482cb7ac1f6f096650db64ae340b273b5aec3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084673"
---
# <a name="deviceinfo-resource-type"></a>Тип ресурса deviceInfo

Пространство имен: microsoft.graph.callRecords

Представляет сведения об устройстве (микрофоне, динамике, камере и т.д.), используемом в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|captureDeviceDriver|Строка|Имя драйвера устройства захвата, используемого конечной точкой мультимедиа.|
|captureDeviceName|Строка|Имя устройства захвата, используемого конечной точкой мультимедиа.|
|captureNotFunctioningEventRatio|Двойное с плавающей точкой|Часть вызова, который конечная точка мультимедиа обнаружила устройство захвата, не работает должным образом.|
|cpuInsufficentEventRatio|Двойное с плавающей точкой|Доля вызова, обнаруживаемого конечной точкой мультимедиа, имеющихся ресурсов ЦП, была недостаточной и привела к низкому качеству звука, отправленного и полученного.|
|deviceClippingEventRatio|Двойное с плавающей точкой|Часть вызова, который конечная точка мультимедиа обнаружила вырезка в захваченном звуке, что привело к плохому качеству отосланного звука.|
|deviceGlitchEventRatio|Двойное с плавающей точкой|Часть вызова, который конечная точка мультимедиа обнаружила сбои или пробелы в аудиозаписи, которые вызывали плохое качество отосланного или полученного звука.|
|howlingEventCount|Int32|Количество раз во время вызова, когда конечная точка мультимедиа обнаружила воение или визг звука.|
|initialSignalLevelRootMeanSquare|Двойное с плавающей точкой|Корневой квадрат (RMS) входящих сигналов до первых 30 секунд вызова.|
|lowSpeechLevelEventRatio|Двойное с плавающей точкой|Часть вызова, в результате чего конечная точка мультимедиа обнаружила низкий уровень речи, что привело к плохому качеству отосланного звука.|
|lowSpeechToNoiseEventRatio|Двойное с плавающей точкой|Часть вызова, который конечная точка мультимедиа обнаружила с низкой речью до уровня шума, что привело к плохому качеству отосланного звука.|
|micGlitchRate|Двойное с плавающей точкой|Сбои в интервале 5 минут для микрофона конечной точки мультимедиа.|
|receivedNoiseLevel|Int32|Средний уровень энергии полученного звука для звука, классифицируется как моношум или левый канал стереошума по конечной точке мультимедиа.|
|receivedSignalLevel|Int32|Средний уровень энергии полученного звука для звука, классифицируется как моноречие, или левый канал стереоречия в конечной точке мультимедиа.|
|renderDeviceDriver|Строка|Имя драйвера устройства визуализации, используемого конечной точкой мультимедиа.|
|renderDeviceName|Строка|Имя устройства визуализации, используемого конечной точкой мультимедиа.|
|renderMuteEventRatio|Двойное с плавающей точкой|Часть вызова, обнаруженного в конечной точке мультимедиа, отключается.|
|renderNotFunctioningEventRatio|Двойное с плавающей точкой|Часть вызова, обнаруживаемого конечной точкой мультимедиа, устройство визуализации не работало должным образом.|
|renderZeroVolumeEventRatio|Двойное с плавающей точкой|Доля тома отображения устройства, обнаруженного конечной точкой мультимедиа, составляет 0.|
|sentNoiseLevel|Int32|Средний уровень энергии отправленного звука для звука, классифицируется как моношум или левый канал стереошума в конечной точке мультимедиа.|
|sentSignalLevel|Int32|Средний уровень энергии отправленного звука для звука, классифицируется как моноречие, или левый канал стереоречия конечной точкой мультимедиа.|
|speakerGlitchRate|Двойное с плавающей точкой|Глюки в 5-минутный внутренний для громкоговоритель конечной точки мультимедиа.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
