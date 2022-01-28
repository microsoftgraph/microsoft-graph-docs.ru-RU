---
title: тип ресурса teamworkSpeakerConfiguration
description: Представляет сведения о конфигурации динамика для Комнаты Microsoft Teams устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88c15b97ea1b2d3984f8e3c3c4a41873fc228ad0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262521"
---
# <a name="teamworkspeakerconfiguration-resource-type"></a>тип ресурса teamworkSpeakerConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации динамика для Комнаты Microsoft Teams [устройства](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isCommunicationSpeakerOptional|Логическое|`True` если динамик связи необязателен. Используется для вычисления состояния здоровья, если динамик связи не является необязательным.|
|isSpeakerOptional|Логическое|`True` если настроенный динамик необязателен. Используется для вычисления состояния здоровья, если динамик не является необязательным.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|defaultCommunicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|Динамик связи по умолчанию, используемый для собраний конференций.|
|defaultSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|Динамик по умолчанию, используемый для всех звуков мультимедиа и уведомлений.|
|динамики|[teamworkPeripheral](../resources/teamworkperipheral.md) collection|Список подключенных динамиков.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSpeakerConfiguration",
  "isCommunicationSpeakerOptional": "Boolean",
  "isSpeakerOptional": "Boolean"
}
```

