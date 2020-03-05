---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 230d688429bb98361c04ad3d28789e0e886361fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529446"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>Тип ресурса Ретиресчедуледманажеддевице

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedDevices, для которых запланировано снятие с учета

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|манажеддевицеид|String|Управляемый DeviceId|
|managedDeviceName|String|Управляемое имя устройства|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Тип устройства управляемого устройства. Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`|
|complianceState|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Управляемое устройство Комплианцестатус. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|ретиреафтердатетиме|DateTimeOffset|Прекращение использования управляемого устройства после даты и времени|
|managementAgent|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|Управляемое устройство Манажементаженттипе. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Управляемое устройство Манажеддевицеовнертипе. Возможные значения: `unknown`, `company`, `personal`.|
|девицекомплианцеполицинаме|String|Имя политики соответствия требованиям устройств|
|девицекомплианцеполициид|String|Соответствие требованиям устройств Полициид|

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
  "deviceCompliancePolicyId": "String"
}
```



