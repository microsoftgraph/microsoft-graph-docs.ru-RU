---
title: тип ресурса teamworkMicrophoneConfiguration
description: Представляет сведения о конфигурации микрофона для Комнаты Microsoft Teams устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cd24375f573e9ff57a0cf9786aee26b1e0826c7c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262518"
---
# <a name="teamworkmicrophoneconfiguration-resource-type"></a>тип ресурса teamworkMicrophoneConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации микрофона для Комнаты Microsoft Teams [устройства](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isMicrophoneOptional|Логическое|`True` если настроенный микрофон необязателен. `False` если микрофон не является необязательным и необходимо вычислить состояние здоровья устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|defaultMicrophone|[teamworkPeripheral](../resources/teamworkperipheral.md)|Сведения о микрофоне по умолчанию.|
|микрофоны|[teamworkPeripheral](../resources/teamworkperipheral.md) collection|Коллекция микрофонов.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkMicrophoneConfiguration",
  "isMicrophoneOptional": "Boolean"
}
```

