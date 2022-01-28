---
title: тип ресурса teamworkDisplayScreenConfiguration
description: Представляет сведения о конфигурации экрана отображения для устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2346de5fa301d1b2db7fd50e4a64c7168eea8a47
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262507"
---
# <a name="teamworkdisplayscreenconfiguration-resource-type"></a>тип ресурса teamworkDisplayScreenConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о конфигурации экрана отображения для устройства с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|backlightBrightness|Int32|Уровень яркости на устройстве (0-100). Не применяется для Комнаты Microsoft Teams устройств.|
|backlightTimeout|Длительность|Время от времени для подсветки (30-3600 сек). Не применяется для Комнаты Teams устройств.|
|isHighContrastEnabled|Логическое|`True` если включен режим высокой контрастности. Не применяется для Комнаты Teams устройств.|
|isScreensaverEnabled|Логическое|`True` если экранный засейвер включен. Не применяется для Комнаты Teams устройств.|
|screensaverTimeout|Длительность|Время на экране от 30 до 3600 секунд. Не применяется для Комнаты Teams устройств.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayScreenConfiguration",
  "backlightBrightness": "Integer",
  "backlightTimeout": "String (duration)",
  "isHighContrastEnabled": "Boolean",
  "isScreensaverEnabled": "Boolean",
  "screensaverTimeout": "String (duration)"
}
```

