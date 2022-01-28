---
title: тип ресурса teamworkTeamsClientConfiguration
description: Представляет сведения о конфигурации для Microsoft Teams клиента, запущенного на Комнаты Microsoft Teams устройстве.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 46c1ac98c9992df65441dd3b92e12f81ae8804b0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262747"
---
# <a name="teamworkteamsclientconfiguration-resource-type"></a>тип ресурса teamworkTeamsClientConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации для Microsoft Teams клиента, запущенного на Комнаты Microsoft Teams [устройстве](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accountConfiguration|[teamworkAccountConfiguration](../resources/teamworkaccountconfiguration.md)|Конфигурация учетной записи Microsoft Teams клиента для устройства.|
|featuresConfiguration|[teamworkFeaturesConfiguration](../resources/teamworkfeaturesconfiguration.md)|Конфигурация Microsoft Teams клиентских функций для устройства.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTeamsClientConfiguration",
  "accountConfiguration": {
    "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
  },
  "featuresConfiguration": {
    "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
  }
}
```

