---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: Аналитика пользовательского интерфейса Work From Anywhere metrics devices summary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffcda6267262de61773d22344d3995279f7d092c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783927"
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
  }
}
```



