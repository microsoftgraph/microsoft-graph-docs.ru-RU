---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: Аналитика пользовательского интерфейса Work From Anywhere metrics devices summary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f63c579739744f897dd0eaa20e4b53cc75aa966a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335616"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsWorkFromAnywhereDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательского интерфейса Work From Anywhere metrics devices summary.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|autopilotDevicesSummary|[userExperienceAnalyticsAutopilotDevicesSummary](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|Значение работы из любого сводки устройств автопилота.|
|cloudManagementDevicesSummary|[userExperienceAnalyticsCloudManagementDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.|
|windows10DevicesSummary|[userExperienceAnalyticsWindows10DevicesSummary](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|Аналитика пользовательских интерфейсов работает из любой Windows 10 устройств.|
|cloudIdentityDevicesSummary|[userExperienceAnalyticsCloudIdentityDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudidentitydevicessummary.md)|Аналитика пользовательских интерфейсов работает из любой сводки устройств облачной идентификации.|
|totalDevices|Int32|Общее количество устройств. Допустимые значения 2147483648 2147483647|
|coManagedDevices|Int32|Общее количество совместно управляемых устройств. Допустимые значения 2147483648 2147483647|
|intuneDevices|Int32|Количество устройств intune, которые не зарегистрированы автопилотом. Допустимые значения 2147483648 2147483647|
|tenantAttachDevices|Int32|Общее количество устройств присоединений клиента. Допустимые значения 2147483648 2147483647|
|windows10Devices|Int32|Количество устройств Windows 10. Допустимые значения 2147483648 2147483647|
|windows10DevicesWithoutTenantAttach|Int32|Количество устройств с Windows 10, которые являются Intune и Comanaged. Допустимые значения 2147483648 2147483647|
|unsupportedOSversionDevices|Int32|Количество устройств Windows 10 с неподтверченными версиями ОС. Допустимые значения 2147483648 2147483647|
|devicesWithoutCloudIdentity|Int32|Количество устройств, не относяющихся к облачной идентификации. Допустимые значения 2147483648 2147483647|
|devicesNotAutopilotRegistered|Int32|Количество устройств intune, которые не зарегистрированы автопилотом. Допустимые значения 2147483648 2147483647|
|devicesWithoutAutopilotProfileAssigned|Int32|Количество устройств intune, не назначенное профилем автопилота. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
  "autopilotDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
    "devicesNotAutopilotRegistered": 1024,
    "devicesWithoutAutopilotProfileAssigned": 1024,
    "totalWindows10DevicesWithoutTenantAttached": 1024
  },
  "cloudManagementDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
    "coManagedDeviceCount": 1024,
    "intuneDeviceCount": 1024,
    "tenantAttachDeviceCount": 1024
  },
  "windows10DevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
    "unsupportedOSversionDeviceCount": 1024
  },
  "cloudIdentityDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
    "deviceWithoutCloudIdentityCount": 1024
  },
  "totalDevices": 1024,
  "coManagedDevices": 1024,
  "intuneDevices": 1024,
  "tenantAttachDevices": 1024,
  "windows10Devices": 1024,
  "windows10DevicesWithoutTenantAttach": 1024,
  "unsupportedOSversionDevices": 1024,
  "devicesWithoutCloudIdentity": 1024,
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




