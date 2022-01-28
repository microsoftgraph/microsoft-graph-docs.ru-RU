---
title: тип ресурса teamworkSystemConfiguration
description: Представляет сведения о конфигурации системы для устройства с Microsoft Teams включенной системой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd22015f77cb65d2be52da8877f9808b73e2cac1
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262585"
---
# <a name="teamworksystemconfiguration-resource-type"></a>тип ресурса teamworkSystemConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации системы для устройства с Microsoft Teams включенной [системой](../resources/teamworkdevice.md). Не применяется для Комнаты Microsoft Teams устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dateTimeConfiguration|[teamworkDateTimeConfiguration](../resources/teamworkdatetimeconfiguration.md)|Конфигурации даты и времени для устройства.|
|defaultPassword|String|Пароль по умолчанию для устройства. Только для записи.|
|deviceLockTimeout|Длительность|Время блокировки устройства в секундах.|
|isDeviceLockEnabled|Логическое|`True` если блокировка устройства включена.|
|isLoggingEnabled|Логическое|`True` если журнал включен.|
|isPowerSavingEnabled|Логическое|`True` если включена экономия электроэнергии.|
|isScreenCaptureEnabled|Логическое|`True` если включен захват экрана.|
|isSilentModeEnabled|Логическое|`True` если включен режим бесшумного режима.|
|language|String|Параметр языка для устройства.|
|lockPin|String|Пин-код, который разблокирует устройство. Только для записи.|
|loggingLevel|String|Уровень ведения журнала для устройства.|
|networkConfiguration|[teamworkNetworkConfiguration](../resources/teamworknetworkconfiguration.md)|Конфигурация сети для устройства.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSystemConfiguration",
  "dateTimeConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
  },
  "defaultPassword": "String",
  "deviceLockTimeout": "String (duration)",
  "isDeviceLockEnabled": "Boolean",
  "isLoggingEnabled": "Boolean",
  "isPowerSavingEnabled": "Boolean",
  "isScreenCaptureEnabled": "Boolean",
  "isSilentModeEnabled": "Boolean",
  "language": "String",
  "lockPin": "String",
  "loggingLevel": "String",
  "networkConfiguration": {
    "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
  }
}
```

