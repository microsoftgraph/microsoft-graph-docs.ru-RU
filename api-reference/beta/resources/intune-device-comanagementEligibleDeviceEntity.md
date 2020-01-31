---
title: Тип ресурса Команажементелигибледевицеентити
description: Тип ресурса Команажементелигибледевицеентити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5ad068a348eabaceafd9ca736f27cf6fda3218e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636555"
---
# <a name="comanagementeligibledeviceentity-resource-type"></a>Тип ресурса Команажементелигибледевицеентити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние конфигурации мобильного приложения для управляемого устройства для данного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Команажементелигибледевицеентити](../api/intune-device-comanagementEligibleDeviceEntity-list.md)|Коллекция [команажементелигибледевицеентити](../resources/intune-device-comanagementEligibleDeviceEntity.md)|Список свойств и связей объектов [команажементелигибледевицеентити](../resources/intune-device-comanagementEligibleDeviceEntity.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор Елигибледевицеентити|
|deviceId|Строка|Устройства|
|deviceName|Строка|DeviceName|
|deviceType|String|DeviceType|
|клиентрегистратионстатус|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Клиентрегистратионстатус. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Возможные значения: `unknown`, `company`, `personal`.|
|managementAgents|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|Манажементаженттипе. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|манажементстате|[манажементстате](../resources/intune-devices-managementstate.md)|Манажементстате. Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|референцеид|Строка|ReferenceId|
|мдмстатус|Строка|мдмстатус|
|osVersion|Строка|OSVersion|
|serialNumber|String|SerialNumber|
|manufacturer|Строка|Вычислитель|
|model|Строка|Модель|
|osDescription|Строка|Свойства OSDescription|
|ентитисаурце|Int32|ентитисаурце|
|userId|String|ИД пользователя|
|Основное|Строка|UPN|
|userEmail|Строка|Электронный адрес пользователя|
|userName|Строка|Имя пользователя|
|команажеелигиблестатус|[команажементелигиблетипе](../resources/intune-devices-comanagementeligibletype.md)|Команажементелигиблетипе. Возможные значения: `coManaged`, `eligible`, `eligibleButNotAadJoined`, `needsOSUpdate`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDeviceEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
  "id": "String (identifier)",
  "deviceId": "String",
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
  "coManageEligibleStatus": "String"
}
```

