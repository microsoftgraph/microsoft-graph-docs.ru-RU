---
title: тип ресурса teamworkDeviceSoftwareVersions
description: Представляет сведения о версиях программного обеспечения для Microsoft Teams устройства с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0605b526e6e3fb3536d1a2fb7c2c14430a8309ed
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262513"
---
# <a name="teamworkdevicesoftwareversions-resource-type"></a>тип ресурса teamworkDeviceSoftwareVersions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о версиях программного обеспечения для устройства с [Microsoft Teams, включая](../resources/teamworkdevice.md) прошивку, операционную систему, Microsoft Teams клиента и агента администрирования.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|adminAgentSoftwareVersion|String|Версия программного обеспечения для агента администрирования, запущенного на устройстве.|
|firmwareSoftwareVersion|String|Версия программного обеспечения для программного обеспечения, запущенного на устройстве.|
|operatingSystemSoftwareVersion|String|Версия программного обеспечения для операционной системы на устройстве.|
|partnerAgentSoftwareVersion|String|Версия программного обеспечения для агента-партнера, запущенного на устройстве.|
|teamsClientSoftwareVersion|String|Версия программного обеспечения для Teams клиента, запущенного на устройстве.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceSoftwareVersions",
  "adminAgentSoftwareVersion": "String",
  "firmwareSoftwareVersion": "String",
  "operatingSystemSoftwareVersion": "String",
  "partnerAgentSoftwareVersion": "String",
  "teamsClientSoftwareVersion": "String"
}
```

