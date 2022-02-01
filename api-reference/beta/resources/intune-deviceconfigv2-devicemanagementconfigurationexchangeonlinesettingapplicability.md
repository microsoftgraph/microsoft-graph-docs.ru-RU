---
title: тип ресурса deviceManagementConfigurationExchangeOnlineSettingApplicability
description: Применимость для параметра Exchange Online
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91d91638865b56044838cd6ff16e741e9949d23a
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291971"
---
# <a name="devicemanagementconfigurationexchangeonlinesettingapplicability-resource-type"></a>тип ресурса deviceManagementConfigurationExchangeOnlineSettingApplicability

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Применимость для параметра Exchange Online


Наследует [от deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|описание параметра Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|платформа|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Параметр платформы можно применять на унаследованной от [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Режим устройства, который можно применить на унаследованной от [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `kiosk`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Какие технологические каналы этого параметра можно развернуть с помощью [inherited from deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```




