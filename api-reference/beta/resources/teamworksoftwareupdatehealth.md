---
title: тип ресурса teamworkSoftwareUpdateHealth
description: Представляет сведения об обновлениях программного обеспечения, доступных для различных компонентов, таких как агент администратора, портал компании, прошивка, операционная система, агент Microsoft Teams и клиент Microsoft Teams устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac1ab4746c83bbcae613c723e1e38ba5f085b4e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262621"
---
# <a name="teamworksoftwareupdatehealth-resource-type"></a>тип ресурса teamworkSoftwareUpdateHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обновлениях программного обеспечения, доступных для различных компонентов, таких как агент администратора, портал компании, прошивка, операционная система, агент партнеров и Microsoft Teams клиент, на устройстве с Microsoft Teams [включенной системой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|adminAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения для агента администрирования.|
|companyPortalSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения, доступное для портала компании.|
|firmwareSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения, доступное для прошивки.|
|operatingSystemSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения для операционной системы.|
|partnerAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения, доступное агенту-партнеру.|
|teamsClientSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|Обновление программного обеспечения, доступное для Teams клиента.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateHealth",
  "adminAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "companyPortalSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "firmwareSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "operatingSystemSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "partnerAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "teamsClientSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  }
}
```

