---
title: тип ресурса retireScheduledManagedDevice
description: ManagedDevices, запланированные к отставку
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1cdbb9009ae55f003e727f949b1d5abe0aad1c6d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821139"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>тип ресурса retireScheduledManagedDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedDevices, запланированные к отставку

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|managedDeviceId|String|Управляемый deviceId|
|managedDeviceName|String|Имя управляемого устройства|
|deviceType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|Тип управляемого устройства. Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` . `unknown`|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Управляемое устройство ComplianceStatus. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|retireAfterDateTime|DateTimeOffset|Управляемые устройства уйдут после даты|
|managementAgent|[managementAgentType](../resources/intune-deviceconfig-managementagenttype.md)|Управление управляемыми устройствамиAgentType. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md).|Управляемое устройство ManagedDeviceOwnerType. Возможные значения: `unknown`, `company`, `personal`.|
|deviceCompliancePolicyName|String|Имя политики соответствия требованиям устройств|
|deviceCompliancePolicyId|String|Политика соответствия требованиям устройств|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



