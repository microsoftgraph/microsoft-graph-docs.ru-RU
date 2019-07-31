---
title: Тип ресурса Виндовсманажеддевице
description: Устройства Windows, которые управляются или предварительно зарегистрированы в Intune
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c3cdc65f53e79bf5a9bb5b31e1438d74ccc876f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999411"
---
# <a name="windowsmanageddevice-resource-type"></a>Тип ресурса Виндовсманажеддевице

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Уникальный идентификатор устройства, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством, унаследованным от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Имя устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Hardwareinformation.|[Hardwareinformation.](../resources/intune-devices-hardwareinformation.md)|Сведения о хардвард для устройства.  Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|Владение устройством. Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Владение устройством. Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Манажементстате|[Манажементстате](../resources/intune-devices-managementstate.md)|Состояние управления для устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Чассистипе|[Чассистипе](../resources/intune-devices-chassistype.md)|Тип корпуса устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Платформа устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[Манажементаженттипе](../resources/intune-devices-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|osVersion|String|Версия операционной системы устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Аадрегистеред|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|Лостмодестате|[Лостмодестате](../resources/intune-devices-lostmodestate.md)|Указывает, включен ли режим потерянных или отключенных наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Сообщения электронной почты пользователя, связанного с устройством, унаследованным из [managedDevice](../resources/intune-devices-manageddevice.md)|
|Свойства azureactivedirectorydeviceid|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемое имя категории устройств, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Защищенное состояние устройства унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[Девицеманажементексчанжеакцессстате](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[Девицеманажементексчанжеакцессстатереасон](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Состояние шифрования устройства, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Имя участника пользователя устройства, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|Модель устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)|
|manufacturer|String|Производитель устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI унаследованы от [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройства, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|Строка|SerialNumber, наследуемый от [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Номер телефона устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Уровень обновления для системы безопасности Android, наследуемый от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Отображаемое имя пользователя, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, поддерживающие клиент Конфигрмгр, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|MAC-адрес сети Wi-Fi, наследуемый от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Оператор перевозчика абонента, наследуемый от [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Общий объем хранилища в байтах, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Свободное хранилище в байтах, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[Манажеддевицепартнеррепортедхеалсстате](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|Ретиреафтердатетиме|DateTimeOffset|Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Усерслогжедон|Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)|Указывает последнего вошедшего в систему пользователей устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Префермдмоверграупполициапплиеддатетиме|DateTimeOffset|Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.  Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики. Только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Аутопилотенроллед|Boolean|Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Рекуиреусеренроллментаппровал|Boolean|Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Манажементцертификатикспиратиондате|DateTimeOffset|Дата окончания срока действия сертификата управления устройствами наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|икЦид|String|Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|удид|String|Уникальный идентификатор устройства для устройств iOS и macOS. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Виндовсактивемалварекаунт|Int32|Число активных вредоносных программ для этого устройства Windows, унаследованных из [managedDevice](../resources/intune-devices-manageddevice.md)|
|Виндовсремедиатедмалварекаунт|Int32|Количество исправленных вредоносных программ для этого устройства Windows, унаследованных из [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
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
  }
}
```





