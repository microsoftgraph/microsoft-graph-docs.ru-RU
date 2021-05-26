---
title: тип ресурса deviceManagementConfigurationWindowsSettingApplicability
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2302bcbae4af684efc159f269d639c50aeb99191
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666683"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>тип ресурса deviceManagementConfigurationWindowsSettingApplicability

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследует [от deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|описание параметра Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|платформа|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Параметр платформы можно применять на унаследованной от [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Режим устройства, который можно применить в режиме Inherited from [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) Возможные значения: `none`, `kiosk`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Какие технологические каналы этого параметра можно развернуть с помощью inherited from [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.|
|configurationServiceProviderVersion|Строка|Версия параметра CSP является частью|
|maximumSupportedVersion|Строка|Максимально поддерживаемая версия Windows|
|minimumSupportedVersion|Строка|Минимальная поддерживаемая версия Windows|
|windowsSkus|[коллекция deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)|Список Windows, применимых к этому параметру|
|requiresAzureAd|Логический|Требование параметра AzureAD|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|Необходимый тип доверия AzureAD. Возможные значения: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.|

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




