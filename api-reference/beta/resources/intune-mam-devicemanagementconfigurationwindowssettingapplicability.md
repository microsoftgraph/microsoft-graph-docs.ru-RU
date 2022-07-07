---
title: Тип ресурса deviceManagementConfigurationWindowsSettingApplicability
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e82561136e1706b5b4fd059dee0d33a15d13836e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66672016"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>Тип ресурса deviceManagementConfigurationWindowsSettingApplicability

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследует от [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|описание параметра Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)|
|платформа|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|Параметр платформы можно применить к inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-shared-devicemanagementconfigurationdevicemode.md)|Режим устройства, который можно применить к inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `kiosk`.|
|Технологии|[deviceManagementConfigurationTechnologies](../resources/intune-mam-devicemanagementconfigurationtechnologies.md)|Какие технологические каналы этого параметра можно развернуть с помощью inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|configurationServiceProviderVersion|String|Версия параметра CSP является частью|
|maximumSupportedVersion|String|Максимальная поддерживаемая версия Windows|
|minimumSupportedVersion|String|Минимальная поддерживаемая версия Windows|
|windowsSkus|[Коллекция deviceManagementConfigurationWindowsSkus](../resources/intune-shared-devicemanagementconfigurationwindowsskus.md)|Список номеров SKU Windows, для которых применим этот параметр|
|requiresAzureAd|Логическое|Требование к настройке AzureAD|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-shared-devicemanagementconfigurationazureadtrusttype.md)|Требуемый тип доверия AzureAD. Возможные значения: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```




