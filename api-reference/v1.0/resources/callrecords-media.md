---
title: тип медиаресумов
description: Тип мультимедиа
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae62d0a6fb05a570bff43f9a92757a429693d4e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025554"
---
# <a name="media-resource-type"></a>тип медиаресумов

Пространство имен: microsoft.graph.callRecords

Представляет носители (аудио, видео, видеосвязь и т.д.), используемые в вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|подпись|Строка|Как были определены средства массовой информации на стадии переговоров.|
|callerDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|Сведения об устройстве, связанные с конечной точкой вызываемого средства массовой информации.|
|callerNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|Сетевые сведения, связанные с конечной точкой вызываемого средства массовой информации.|
|calleeDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|Сведения об устройстве, связанные с конечной точкой вызова этого носитеса.|
|calleeNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|Сетевые сведения, связанные с конечной точкой вызова этого носитела.|
|потоки|[коллекция microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md)|Сетевые потоки, связанные с этим мультимедиа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
