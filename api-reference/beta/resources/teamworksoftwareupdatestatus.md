---
title: тип ресурса teamworkSoftwareUpdateStatus
description: Представляет сведения о состоянии обновления программного обеспечения для различных компонентов, таких как агент администрирования, портал компании, прошивка, операционная система, агент партнеров и клиент Microsoft Teams, на устройстве с Microsoft Teams включенной системой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a50046c758db26ae1d53507263c65dba7aff7435
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262615"
---
# <a name="teamworksoftwareupdatestatus-resource-type"></a>тип ресурса teamworkSoftwareUpdateStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии обновления программного обеспечения для различных компонентов, таких как агент администратора, портал компании, прошивка, операционная система, агент партнеров и клиент Microsoft Teams, на устройстве с Microsoft Teams [включенной системой](../resources/teamworkdevice.md). Он указывает, требуется ли обновление программного обеспечения или нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|availableVersion|String|Доступная версия программного обеспечения для обновления.|
|currentVersion|String|Текущая версия программного обеспечения.|
|softwareFreshness|teamworkSoftwareFreshness|Состояние обновления программного обеспечения. Допустимые значения: `unknown`, `latest`, `updateAvailable`, `unknownFutureValue`.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateStatus",
  "availableVersion": "String",
  "currentVersion": "String",
  "softwareFreshness": "String"
}
```

