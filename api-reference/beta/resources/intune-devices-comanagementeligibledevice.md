---
title: Тип ресурса comanagementEligibleDevice
description: Состояние Co-Management устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d9c17a3de8a1b2d3bf30874f0202cf432447ef6
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670823"
---
# <a name="comanagementeligibledevice-resource-type"></a>Тип ресурса comanagementEligibleDevice

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние Co-Management устройств

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление comanagementEligibleDevices](../api/intune-devices-comanagementeligibledevice-list.md)|[Коллекция comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Список свойств и связей объектов [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Получение comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-get.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Чтение свойств и связей объекта [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Создание comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-create.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Создайте объект [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Удаление comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-delete.md)|Нет|Удаляет [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).|
|[Обновление comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-update.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Обновление свойств объекта [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства|
|deviceName|String|DeviceName|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|DeviceType. Возможные значения: `desktop`, , `windowsRT``winMO6`, `nokia`, `windowsPhone`, `holoLens``macMDM``winCE``winEmbedded``mac``iPhone``iPod``android``iPad``androidForWork``unix``surfaceHub``iSocConsumer``androidEnterprise`, `chromeOS``windows10x``androidnGMS``linux`, , , `blackberry`, . `palm``unknown``cloudPC`|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Возможные значения: `unknown`, `company`, `personal`.|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgents. Возможные значения: `eas`, , `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient``configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf``googleCloudDevicePolicyController`, , `microsoft365ManagedMdm`, . `msSense``intuneAosp`|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|ManagementState. Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|referenceId|String|ReferenceId|
|mdmStatus|String|MDMStatus|
|osVersion|String|OSVersion|
|serialNumber|String|SerialNumber|
|manufacturer|String|Производитель|
|model|String|Модель|
|osDescription|String|Описание OSDescription|
|entitySource|Int32|EntitySource|
|userId|String|ИД пользователя|
|Upn|String|Имя участника-пользователя|
|userEmail|String|Электронный адрес пользователя|
|userName|String|Имя пользователя|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|ComanagementEligibleStatus. Возможные значения: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceType": "String",
  "clientRegistrationStatus": "String",
  "ownerType": "String",
  "managementAgents": "String",
  "managementState": "String",
  "referenceId": "String",
  "mdmStatus": "String",
  "osVersion": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "osDescription": "String",
  "entitySource": 1024,
  "userId": "String",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "status": "String"
}
```




