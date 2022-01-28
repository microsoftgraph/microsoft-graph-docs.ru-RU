---
title: тип ресурса teamworkHardwareHealth
description: Представляет сведения о оборудовании устройства, Microsoft Teams включенного устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc552dc46199e1107220ae6ed27c839126e4888f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262526"
---
# <a name="teamworkhardwarehealth-resource-type"></a>тип ресурса teamworkHardwareHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о оборудовании устройства, Microsoft Teams включенного [устройства](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|computeHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о состоянии системы для [teamworkDevice](../resources/teamworkdevice.md).|
|hdmiIngestHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Сведения о том, как hdMI гнается на устройстве.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareHealth",
  "computeHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "hdmiIngestHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  }
}
```

