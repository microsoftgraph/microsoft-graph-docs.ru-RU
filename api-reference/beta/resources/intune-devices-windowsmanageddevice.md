---
title: Тип ресурса Виндовсманажеддевице
description: Устройства Windows, которые управляются или предварительно зарегистрированы в Intune
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 170579d94b5c28e2c77c404d18a408322f8d8c4f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783622"
---
# <a name="windowsmanageddevice-resource-type"></a>Тип ресурса Виндовсманажеддевице

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройства Windows, которые управляются или предварительно зарегистрированы в Intune


Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсманажеддевицес](../api/intune-devices-windowsmanageddevice-list.md)|Коллекция [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md)|Список свойств и связей объектов [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .|
|[Получение Виндовсманажеддевице](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Чтение свойств и связей объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .|
|[Создание Виндовсманажеддевице](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Создание нового объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .|
|[Удаление Виндовсманажеддевице](../api/intune-devices-windowsmanageddevice-delete.md)|Нет|Удаляет объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).|
|[Обновление Виндовсманажеддевице](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Обновление свойств объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Имя устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Hardwareinformation.|[Hardwareinformation.](../resources/intune-devices-hardwareinformation.md)|Сведения о хардвард для устройства.  Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Владение устройством. Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Владение устройством. Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|манажементстате|[манажементстате](../resources/intune-devices-managementstate.md)|Состояние управления для устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|чассистипе|[чассистипе](../resources/intune-devices-chassistype.md)|Тип корпуса устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Платформа устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|osVersion|String|Версия операционной системы устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Логический|Указывает, активировано ли устройство в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|аадрегистеред|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.|
|лостмодестате|[лостмодестате](../resources/intune-devices-lostmodestate.md)|Указывает, включен ли режим потерянных или отключенных. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Сообщения электронной почты пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Свойства azureactivedirectorydeviceid|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемое имя категории устройств. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Состояние контролируемого устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[девицеманажементексчанжеакцессстате](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[девицеманажементексчанжеакцессстатереасон](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Состояние шифрования устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Имя участника пользователя устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|Модель устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|manufacturer|String|Производитель устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройства требованиям. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|Строка|Серийный. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Номер телефона устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Уровень обновления для системы безопасности Android. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Отображаемое имя пользователя. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, поддерживающие клиент Конфигрмгр. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|MAC Wi-Fi. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Перевозчик абонента. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Общий объем хранилища в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Свободное хранилище в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[манажеддевицепартнеррепортедхеалсстате](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|ретиреафтердатетиме|DateTimeOffset|Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|усерслогжедон|Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)|Указывает последнего вошедшего в систему пользователя устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|префермдмоверграупполициапплиеддатетиме|DateTimeOffset|Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.  Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|аутопилотенроллед|Логический|Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|рекуиреусеренроллментаппровал|Логический|Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|манажементцертификатикспиратиондате|DateTimeOffset|Дата окончания срока действия сертификата управления устройствами. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|икЦид|String|Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|удид|String|Уникальный идентификатор устройства для устройств iOS и macOS. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого экземпляра устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|виндовсактивемалварекаунт|Int32|Количество активных вредоносных программ для этого устройства Windows. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|виндовсремедиатедмалварекаунт|Int32|Количество исправленных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)|
|есернетмакаддресс|String|MAC Ethernet. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|фисикалмеморинбитес|Int64|Общий объем памяти в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|процессорарчитектуре|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Архитектура процессора. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Все приложения, которые установлены на устройстве, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Категория устройства, унаследованная от [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Состояние защиты устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|users|Коллекция объектов [user](../resources/intune-shared-user.md)|Основные пользователи, связанные с управляемым устройством. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String",
    "isBlocked": true
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String"
}
```



