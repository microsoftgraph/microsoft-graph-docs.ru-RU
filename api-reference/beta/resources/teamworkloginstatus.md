---
title: тип ресурса teamworkLoginStatus
description: Представляет Microsoft Teams, Skype для бизнеса и Exchange для устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460b9bfb341f7b8a564347f0ab4f64d824120d09
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262711"
---
# <a name="teamworkloginstatus-resource-type"></a>тип ресурса teamworkLoginStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Microsoft Teams, Skype для бизнеса и Exchange для устройства с Microsoft Teams [включенной](../resources/teamworkdevice.md) поддержкой.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ExchangeConnection|[teamworkConnection](../resources/teamworkconnection.md)|Сведения о Exchange подключения.|
|skypeConnection|[teamworkConnection](../resources/teamworkconnection.md)|Сведения о Skype для бизнеса подключения.|
|teamsConnection|[teamworkConnection](../resources/teamworkconnection.md)|Сведения о Teams подключения.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkLoginStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkLoginStatus",
  "exchangeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "teamsConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "skypeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  }
}
```

