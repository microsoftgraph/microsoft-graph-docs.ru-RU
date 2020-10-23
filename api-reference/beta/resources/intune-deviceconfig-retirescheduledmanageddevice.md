---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2939da221a47e878414c5a24f2ed44fdd9c5e238
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729681"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>Тип ресурса Ретиресчедуледманажеддевице

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedDevices, для которых запланировано снятие с учета

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|манажеддевицеид|Строка|Управляемый DeviceId|
|managedDeviceName|String|Управляемое имя устройства|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Тип устройства управляемого устройства. Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.|
|complianceState|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Управляемое устройство Комплианцестатус. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|ретиреафтердатетиме|DateTimeOffset|Прекращение использования управляемого устройства после даты и времени|
|managementAgent|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|Управляемое устройство Манажементаженттипе. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Управляемое устройство Манажеддевицеовнертипе. Возможные значения: `unknown`, `company`, `personal`.|
|девицекомплианцеполицинаме|Строка|Имя политики соответствия требованиям устройств|
|девицекомплианцеполициид|Строка|Соответствие требованиям устройств Полициид|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|

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





