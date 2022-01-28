---
title: тип ресурса teamworkAccountConfiguration
description: Представляет сведения о конфигурации учетной записи для Комнаты Microsoft Teams устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b3fc0edb85380f8a858bf6b9910a819443bfb8b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262602"
---
# <a name="teamworkaccountconfiguration-resource-type"></a>тип ресурса teamworkAccountConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации учетной записи для Комнаты Microsoft Teams [устройства](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|onPremisesCalendarSyncConfiguration|[teamworkOnPremisesCalendarSyncConfiguration](../resources/teamworkonpremisescalendarsyncconfiguration.md)|Учетная запись, используемая для синхронизации календаря.|
|supportedClient|teamworkSupportedClient|Поддерживаемый клиент для Комнаты Teams устройств. Допустимые значения: `unknown`, `skypeDefaultAndTeams`, `teamsDefaultAndSkype`, `skypeOnly`, `teamsOnly`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkAccountConfiguration",
  "onPremisesCalendarSyncConfiguration": {
    "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
  },
  "supportedClient": "String"
}
```

