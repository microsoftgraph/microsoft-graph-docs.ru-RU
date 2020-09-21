---
title: Тип ресурса Команажементелигибледевице
description: Состояние возможности совместного управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6a912aa9631295c7331afa8f1d985b5231ac614
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060764"
---
# <a name="comanagementeligibledevice-resource-type"></a>Тип ресурса Команажементелигибледевице

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние возможности совместного управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Команажементелигибледевицес](../api/intune-devices-comanagementeligibledevice-list.md)|Коллекция [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md)|Список свойств и связей объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Получение Команажементелигибледевице](../api/intune-devices-comanagementeligibledevice-get.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Чтение свойств и связей объекта [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Создание Команажементелигибледевице](../api/intune-devices-comanagementeligibledevice-create.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Создание нового объекта [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Удаление Команажементелигибледевице](../api/intune-devices-comanagementeligibledevice-delete.md)|Нет|Удаляет объект [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md).|
|[Обновление Команажементелигибледевице](../api/intune-devices-comanagementeligibledevice-update.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Обновление свойств объекта [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства|
|deviceName|String|DeviceName|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|DeviceType. Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.|
|клиентрегистратионстатус|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Клиентрегистратионстатус. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Возможные значения: `unknown`, `company`, `personal`.|
|managementAgents|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|ManagementAgents. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|манажементстате|[манажементстате](../resources/intune-devices-managementstate.md)|Манажементстате. Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|референцеид|String|ReferenceId|
|мдмстатус|String|мдмстатус|
|osVersion|String|OSVersion|
|serialNumber|String|SerialNumber|
|manufacturer|String|Вычислитель|
|model|String|Модель|
|osDescription|String|Свойства OSDescription|
|ентитисаурце|Int32|ентитисаурце|
|userId|String|ИД пользователя|
|Основное|String|Имя участника-пользователя|
|userEmail|String|Электронный адрес пользователя|
|userName|String|Имя пользователя|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|Команажементелигиблестатус. Возможные значения: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|

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






