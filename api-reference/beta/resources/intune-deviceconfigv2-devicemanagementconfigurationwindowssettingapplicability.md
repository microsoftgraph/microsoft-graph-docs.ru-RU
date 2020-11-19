---
title: Тип ресурса Девицеманажементконфигуратионвиндовссеттингаппликабилити
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3b520a194a09d178790f5a82f3ca21c1e00d2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301930"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>Тип ресурса Девицеманажементконфигуратионвиндовссеттингаппликабилити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследуется от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание параметра, унаследованного от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|платформа|[девицеманажементконфигуратионплатформс](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Параметр платформы можно применять для наследования от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|девицемоде|[девицеманажементконфигуратиондевицемоде](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Режим устройства, с которым можно применять параметры, наследуемые от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `kiosk`.|
|технологически|[девицеманажементконфигуратионтечнологиес](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Какие технологические каналы этот параметр можно развернуть с помощью наследования от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.|
|конфигуратионсервицепровидерверсион|String|Версия параметра CSP является частью|
|максимумсуппортедверсион|String|Максимальная поддерживаемая версия Windows|
|минимумсуппортедверсион|String|Минимальная поддерживаемая версия Windows|
|виндовсскус|Коллекция [девицеманажементконфигуратионвиндовсскус](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)|Список SKU Windows, к которым применяется параметр|
|рекуиресазуреад|Boolean|Требование к параметру AzureAD|
|рекуиредазуреадтрусттипе|[девицеманажементконфигуратионазуреадтрусттипе](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|Обязательный тип доверия AzureAD. Возможные значения: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.|

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




