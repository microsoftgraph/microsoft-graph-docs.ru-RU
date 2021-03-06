---
title: Тип ресурса managedDevice
description: Устройства, которые управляются или предварительно регистрируются с помощью Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62cc8d092201497d15cb49fb17fcf52f0a64eb6f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161009"
---
# <a name="manageddevice-resource-type"></a>Тип ресурса managedDevice

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройства, которые управляются или предварительно регистрируются с помощью Intune

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedDevice](../api/intune-policyset-manageddevice-list.md)|Коллекция [managedDevice](../resources/intune-shared-manageddevice.md)|Перечисление свойств и связей объектов [managedDevice](../resources/intune-shared-manageddevice.md).|
|[Получение объекта managedDevice](../api/intune-policyset-manageddevice-get.md)|[managedDevice](../resources/intune-shared-manageddevice.md)|Чтение свойств и связей объекта [managedDevice](../resources/intune-shared-manageddevice.md).|
|[Создание объекта managedDevice](../api/intune-policyset-manageddevice-create.md)|[managedDevice](../resources/intune-shared-manageddevice.md)|Создание объекта [managedDevice](../resources/intune-shared-manageddevice.md).|
|[Удаление объекта managedDevice](../api/intune-policyset-manageddevice-delete.md)|Нет|Удаление объекта [managedDevice](../resources/intune-shared-manageddevice.md).|
|[Обновление объекта managedDevice](../api/intune-policyset-manageddevice-update.md)|[managedDevice](../resources/intune-shared-manageddevice.md)|Обновление свойств объекта [managedDevice](../resources/intune-shared-manageddevice.md).|
|[Действие executeAction](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md);|Пока не задокументировано.|
|[Действие enableLostMode](../api/intune-devices-manageddevice-enablelostmode.md)|Нет|Включить режим потери|
|[Действие playLostModeSound](../api/intune-devices-manageddevice-playlostmodesound.md)|Нет|Удаленная блокировка|
|[Действие setDeviceName](../api/intune-devices-manageddevice-setdevicename.md)|Нет|За установите имя устройства.|
|[Действие rotateFileVaultKey](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|Нет|Н/Д|
|[Функция getFileVaultKey](../api/intune-devices-manageddevice-getfilevaultkey.md)|String|Пока не задокументировано.|
|[Действие createDeviceLogCollectionRequest](../api/intune-devices-manageddevice-createdevicelogcollectionrequest.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Пока не задокументировано.|
|[Действие retire](../api/intune-devices-manageddevice-retire.md)|Нет|Прекращение использования устройства|
|[Действие wipe](../api/intune-devices-manageddevice-wipe.md)|Нет|Очистка устройства|
|[Действие resetPasscode](../api/intune-devices-manageddevice-resetpasscode.md)|Нет|Сброс секретного кода|
|[Действие remoteLock](../api/intune-devices-manageddevice-remotelock.md)|Нет|Удаленная блокировка|
|[Действие requestRemoteAssistance](../api/intune-devices-manageddevice-requestremoteassistance.md)|Нет|Запрос удаленной помощи|
|[Действие disableLostMode](../api/intune-devices-manageddevice-disablelostmode.md)|Нет|Отключение режима пропажи устройства|
|[Действие locateDevice](../api/intune-devices-manageddevice-locatedevice.md)|Нет|Поиск устройства|
|[Действие bypassActivationLock](../api/intune-devices-manageddevice-bypassactivationlock.md)|Нет|Обход блокировки активации|
|[Действие rebootNow](../api/intune-devices-manageddevice-rebootnow.md)|Нет|Перезагрузка устройства|
|[Действие shutDown](../api/intune-devices-manageddevice-shutdown.md)|Нет|Завершение работы устройства|
|[Действие recoverPasscode](../api/intune-devices-manageddevice-recoverpasscode.md)|Нет|Восстановление секретного кода|
|[Действие cleanWindowsDevice](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|Нет|Очистка устройства с Windows|
|[Действие logoutSharedAppleDeviceActiveUser](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|Нет|Выход от имени активного пользователя общего устройства Apple|
|[Действие deleteUserFromSharedAppleDevice](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|Нет|Удаление пользователя с общего устройства Apple|
|[Действие syncDevice](../api/intune-devices-manageddevice-syncdevice.md)|Нет|Н/Д|
|[Действие windowsDefenderScan](../api/intune-devices-manageddevice-windowsdefenderscan.md)|Нет|Н/Д|
|[Действие windowsDefenderUpdateSignatures](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|Нет|Н/Д|
|[Действие updateWindowsDeviceAccount](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|Нет|Н/Д|
|[Действие revokeAppleVppLicenses](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|Нет|Отзывать все лицензии Apple VPP для устройства|
|[Действие rotateBitLockerKeys](../api/intune-devices-manageddevice-rotatebitlockerkeys.md)|Нет|Поворот BitLockerKeys|
|[Действие sendCustomNotificationToCompanyPortal](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|Нет|Н/Д|
|[Действие triggerConfigurationManagerAction](../api/intune-devices-manageddevice-triggerconfigurationmanageraction.md)|Нет|Действие триггера для клиента ConfigurationManager|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства. Это свойство доступно только для чтения.|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством. Это свойство доступно только для чтения.|
|deviceName|String|Имя устройства. Это свойство доступно только для чтения.|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Подробные сведения об устройстве.  Включает такие сведения, как место в хранилище, изготовитель, серийный номер и т. д. Это свойство является свойством только для чтения.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Владение устройством. Может быть "company" или "personal". Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Владение устройством. Может быть "company" или "personal". Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Это свойство доступно только для чтения.|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Состояние управления устройством. Это свойство доступно только для чтения. Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Это свойство доступно только для чтения.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Это свойство доступно только для чтения.|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Тип корпусов устройства. Это свойство доступно только для чтения. Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Это свойство находится только для чтения.|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Платформа устройства. Это свойство доступно только для чтения. Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` , `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Это свойство доступно только для чтения.|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Это свойство находится только для чтения. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|osVersion|String|Версия операционной системы устройства. Это свойство доступно только для чтения.|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync. Это свойство доступно только для чтения.|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Это свойство доступно только для чтения.|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Это свойство доступно только для чтения.|
|aadRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения.|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации устройства. Это свойство доступно только для чтения. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Указывает, включен ли режим потери. Это свойство доступно только для чтения. Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Это свойство доступно только для чтения.|
|emailAddress|String|Электронная почта пользователя, связанного с устройством. Это свойство доступно только для чтения.|
|azureActiveDirectoryDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения.|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Это свойство доступно только для чтения. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемая имя категории устройства. Это свойство доступно только для чтения.|
|isSupervised|Boolean|Состояние устройства под контролем. Это свойство доступно только для чтения.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Это свойство доступно только для чтения.|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Это свойство доступно только для чтения. Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Это свойство доступно только для чтения. Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Это свойство доступно только для чтения.|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Это свойство доступно только для чтения.|
|isEncrypted|Boolean|Состояние шифрования устройства. Это свойство доступно только для чтения.|
|userPrincipalName|String|Имя пользователя устройства. Это свойство доступно только для чтения.|
|model|String|Модель устройства. Это свойство доступно только для чтения.|
|manufacturer|String|Производитель устройства. Это свойство доступно только для чтения.|
|imei|String|IMEI. Это свойство доступно только для чтения.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройств требованиям. Это свойство доступно только для чтения.|
|serialNumber|String|SerialNumber. Это свойство доступно только для чтения.|
|phoneNumber|String|Номер телефона устройства. Это свойство доступно только для чтения.|
|androidSecurityPatchLevel|String|Уровень исправлений для системы безопасности Android. Это свойство доступно только для чтения.|
|userDisplayName|String|Отображаемая имя пользователя. Это свойство доступно только для чтения.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, включенные клиентом ConfigrMgr. Это свойство доступно только для чтения.|
|wiFiMacAddress|String|Wi-Fi MAC. Это свойство доступно только для чтения.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Это свойство доступно только для чтения.|
|subscriberCarrier|String|Оператор абонента. Это свойство доступно только для чтения.|
|meid|String|MEID. Это свойство доступно только для чтения.|
|totalStorageSpaceInBytes|Int64|Общее хранилище в bytes. Это свойство доступно только для чтения.|
|freeStorageSpaceInBytes|Int64|Бесплатное хранилище в вайтах. Это свойство доступно только для чтения.|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Это свойство доступно только для чтения. Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Указывает время после автоматического выхода устройства из-за запланированного действия. Это свойство доступно только для чтения.|
|usersLoggedOn|[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)|Указывает последнего во время входа пользователей устройства. Это свойство доступно только для чтения.|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Сообщает dateTime, задав параметр preferMdmOverGroupPolicy.  Если этот параметр задан, параметры MDM Intune будут переопределять параметры групповой политики в случае конфликта. Только для чтения. Это свойство доступно только для чтения.|
|autopilotEnrolled|Boolean|Сообщает, зарегистрировать ли управляемое устройство с помощью автоматического пилотного проекта. Это свойство доступно только для чтения.|
|requireUserEnrollmentApproval|Boolean|Сообщает, является ли управляемое устройство iOS зарегистрированным пользователем. Это свойство доступно только для чтения.|
|managementCertificateExpirationDate|DateTimeOffset|Сообщает дату окончания срока действия сертификата управления устройствами. Это свойство доступно только для чтения.|
|iccid|String|Интегрированный идентификатор схемной карты — это уникальный идентификационный номер SIM-карты. Это свойство доступно только для чтения.|
|udid|String|Уникальный идентификатор устройства для устройств с iOS и macOS. Это свойство доступно только для чтения.|
|roleScopeTagIds|Коллекция String|Список ИД тегов области для этого экземпляра устройства.|
|windowsActiveMalwareCount|Int32|Количество активных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения.|
|windowsRemediatedMalwareCount|Int32|Количество исправленных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения.|
|notes|String|Заметки на устройстве, созданном ИТ-администратором|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние состояния клиента Configuration Manager, действительное только для устройств, управляемых агентом MDM/ConfigMgr|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Сведения о клиенте Configuration Manager, допустимые только для устройств, управляемых, управляемых duel или триуправленных агентом ConfigMgr|
|ethernetMacAddress|String|Ethernet MAC. Это свойство доступно только для чтения.|
|physicalMemoryInBytes|Int64|Общий объем памяти в ветвях. Это свойство доступно только для чтения.|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Архитектура процессора. Это свойство доступно только для чтения. Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|specificationVersion|String|Версия спецификации. Это свойство доступно только для чтения.|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Тип присоединить устройство. Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|skuFamily|String|Семейство SKU устройств|
|skuNumber|Int32|Номер SKU устройства, см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo . Допустимые значения: от 0 до 2 147 483 647. Это свойство доступно только для чтения.|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|Функции управления устройствами. Возможные значения: `none`, `microsoftManagedDesktop`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignmentFilterEvaluationStatusDetails|[Коллекция assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Состояния конфигурации мобильного приложения для управляемого устройства.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Все приложения, установленные на устройстве в данный момент|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Категория устройства|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Состояние защиты устройства.|
|users|Коллекция объектов [user](../resources/intune-shared-user.md)|Основные пользователи, связанные с управляемым устройством.|
|logCollectionRequests|[Коллекция deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Список запросов на сбор журналов|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
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
    "batterySerialNumber": "String",
    "batteryHealthPercentage": 1024,
    "batteryChargeCycles": 1024,
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
    "osBuildNumber": "String",
    "operatingSystemProductType": 1024,
    "ipAddressV4": "String",
    "subnetAddress": "String"
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
  "processorArchitecture": "String",
  "specificationVersion": "String",
  "joinType": "String",
  "skuFamily": "String",
  "skuNumber": 1024,
  "managementFeatures": "String"
}
```



