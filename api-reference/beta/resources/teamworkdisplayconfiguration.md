---
title: тип ресурса teamworkDisplayConfiguration
description: Представляет сведения о конфигурации дисплея для устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88de0c02af3012b1fff55f4ef1cb0f58773c4f7b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262501"
---
# <a name="teamworkdisplayconfiguration-resource-type"></a>тип ресурса teamworkDisplayConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации дисплея для устройства с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|configuredDisplays|[teamworkConfiguredPeripheral](../resources/teamworkconfiguredperipheral.md) collection|Список настроенных дисплеев. Применимо только для Комнаты Microsoft Teams устройств.|
|displayCount|Int32|Общее количество подключенных дисплеев, включая встроенный дисплей. Применимо только для Комнаты Teams устройств.|
|inBuiltDisplayScreenConfiguration|[teamworkDisplayScreenConfiguration](../resources/teamworkdisplayscreenconfiguration.md)|Конфигурация для встроеного дисплея. Не применяется для Комнаты Teams устройств.|
|isContentDuplicationAllowed|Логическое|`True` если допускается дублирование контента. Применимо только для Комнаты Teams устройств.|
|isDualDisplayModeEnabled|Логическое|`True` если включен режим двойного отображения. Если **isDualDisplayModeEnabled** `true`является, то содержимое будет отображаться на обоих экранах комнаты, а не только на одном экране, когда он передается через гнойный модуль HDMI на Комнаты Microsoft Teams устройстве. Применимо только для Комнаты Teams устройств.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayConfiguration",
  "configuredDisplays": [
    {
      "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
    }
  ],
  "displayCount": "Integer",
  "inBuiltDisplayScreenConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
  },
  "isContentDuplicationAllowed": "Boolean",
  "isDualDisplayModeEnabled": "Boolean"
}
```

