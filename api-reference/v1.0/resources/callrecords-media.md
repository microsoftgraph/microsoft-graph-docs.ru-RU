---
title: Тип ресурса мультимедиа
description: Тип мультимедиа
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0eeefd772eb7050a829c7eaf9d65f92958c8fa64
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492047"
---
# <a name="media-resource-type"></a>Тип ресурса мультимедиа

Пространство имен: microsoft.graph.callRecords

Представляет мультимедиа (звук, видео, Видеообмен на экране и т. д.), используемые при вызове.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|label|String|Способ идентификации мультимедиа во время этапа согласования мультимедиа.|
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