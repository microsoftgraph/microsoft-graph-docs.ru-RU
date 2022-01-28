---
title: тип ресурса teamworkPeripheralsHealth
description: Представляет сведения о состоянии здоровья для всех периферийных устройств, подключенных к Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d48c0351a20ed1074f5bb2fd4443d40bf96d52d6
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262632"
---
# <a name="teamworkperipheralshealth-resource-type"></a>тип ресурса teamworkPeripheralsHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии здоровья для всех периферийных устройств, подключенных к Microsoft Teams с [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|communicationSpeakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья динамика связи.|
|contentCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья камеры контента.|
|displayHealthCollection|[коллекция teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья дисплеев.|
|microphoneHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья микрофона.|
|roomCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья камеры комнаты.|
|speakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии здоровья динамика.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralsHealth",
  "communicationSpeakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "contentCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "displayHealthCollection": [
    {
      "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
    }
  ],
  "microphoneHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "roomCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "speakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  }
}
```

