---
title: Тип ресурса retireScheduledManagedDevice
description: ManagedDevices, которые запланированы для прекращения использования
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdc0d2e97c417d0189805006fc6636aaae4b154b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667637"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>Тип ресурса retireScheduledManagedDevice

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedDevices, которые запланированы для прекращения использования

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|managedDeviceId|String|Управляемый идентификатор устройства|
|managedDeviceName|String|Имя управляемого устройства|
|deviceType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|Тип устройства управляемого устройства. Возможные значения: `desktop`, , `windowsRT``winMO6`, `nokia`, `windowsPhone`, `holoLens``macMDM``winCE``winEmbedded``mac``iPhone``iPod``android``iPad``androidForWork``unix``surfaceHub``iSocConsumer``androidEnterprise`, `chromeOS``windows10x``androidnGMS``linux`, , , `blackberry`, . `palm``unknown``cloudPC`|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|ComplianceStatus для управляемых устройств. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|retireAfterDateTime|DateTimeOffset|Прекращение использования управляемого устройства после даты и времени|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Managed Device ManagementAgentType. Возможные значения: `eas`, , `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient``configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf``googleCloudDevicePolicyController`, , `microsoft365ManagedMdm`, . `msSense``intuneAosp`|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md).|Managed Device ManagedDeviceOwnerType. Возможные значения: `unknown`, `company`, `personal`.|
|deviceCompliancePolicyName|String|Имя политики соответствия устройств|
|deviceCompliancePolicyId|String|Идентификатор политики соответствия устройств|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности.|

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




