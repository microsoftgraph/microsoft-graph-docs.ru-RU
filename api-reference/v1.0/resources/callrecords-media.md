---
title: Тип ресурса мультимедиа
description: Тип мультимедиа
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: edd4849cc6922695f7c03909ac04348b4171d5a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069395"
---
# <a name="media-resource-type"></a>Тип ресурса мультимедиа

Пространство имен: microsoft.graph.callRecords

Представляет мультимедиа (звук, видео, Видеообмен на экране и т. д.), используемые при вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|label|Строка|Способ идентификации мультимедиа во время этапа согласования мультимедиа.|
|каллердевице|[Microsoft. Graph. Каллрекордс. Девицеинфо](callrecords-deviceinfo.md)|Сведения об устройстве, связанные с конечной точкой абонента этого носителя.|
|каллернетворк|[Microsoft. Graph. Каллрекордс. Нетворкинфо](callrecords-networkinfo.md)|Сведения о сети, связанные с конечной точкой абонента этого носителя.|
|каллидевице|[Microsoft. Graph. Каллрекордс. Девицеинфо](callrecords-deviceinfo.md)|Сведения об устройстве, связанные с конечной точкой вызываемого носителя.|
|каллинетворк|[Microsoft. Graph. Каллрекордс. Нетворкинфо](callrecords-networkinfo.md)|Сведения о сети, связанные с конечной точкой вызываемого носителя.|
|представлений|Коллекция [Microsoft. Graph. каллрекордс. медиастреам](callrecords-mediastream.md)|Сетевые потоки, связанные с этим носителем.|

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
