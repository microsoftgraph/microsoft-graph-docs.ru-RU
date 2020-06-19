---
title: Тип ресурса managedDevice
description: Устройства, которые управляются или предварительно регистрируются с помощью Intune
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4121162498e3c47aff32667815ad22b6a31453eb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788068"
---
# <a name="manageddevice-resource-type"></a>Тип ресурса managedDevice

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройства, которые управляются или предварительно регистрируются с помощью Intune

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md);|Чтение свойств и связей объекта [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Обновление объекта managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Действие executeAction](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md);|Пока не задокументировано.|
|[Действие enableLostMode](../api/intune-devices-manageddevice-enablelostmode.md)|Нет|Включение режима потери|
|[Действие playLostModeSound](../api/intune-devices-manageddevice-playlostmodesound.md)|Нет|Удаленная блокировка|
|[Действие setDeviceName](../api/intune-devices-manageddevice-setdevicename.md)|Нет|Задание имени устройства для устройства.|
|[действие Ротатефилеваулткэй](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|None|Пока не задокументировано|
|[Функция Жетфилеваулткэй](../api/intune-devices-manageddevice-getfilevaultkey.md)|String|Пока не задокументировано.|
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
|[Действие syncDevice](../api/intune-devices-manageddevice-syncdevice.md)|None|Пока не задокументировано|
|[Действие windowsDefenderScan](../api/intune-devices-manageddevice-windowsdefenderscan.md)|None|Пока не задокументировано|
|[Действие windowsDefenderUpdateSignatures](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|None|Н/Д|
|[Действие updateWindowsDeviceAccount](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|Нет|Пока не задокументировано|
|[Действие revokeAppleVppLicenses](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|Нет|Отзыв всех лицензий на Apple VPP для устройства|
|[действие Ротатебитлоккеркэйс](../api/intune-devices-manageddevice-rotatebitlockerkeys.md)|Нет|Поворот Битлоккеркэйс|
|[Действие sendCustomNotificationToCompanyPortal](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|None|Пока не задокументировано|
|[действие Тригжерконфигуратионманажерактион](../api/intune-devices-manageddevice-triggerconfigurationmanageraction.md)|Нет|Действие триггера в клиенте Конфигуратионманажер|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства. Это свойство доступно только для чтения.|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством. Это свойство доступно только для чтения.|
|deviceName|String|Имя устройства. Это свойство доступно только для чтения.|
|Hardwareinformation.|[Hardwareinformation.](../resources/intune-devices-hardwareinformation.md)|Сведения о хардвард для устройства.  Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Владение устройством. Может быть "Company" или "Personal". Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Владение устройством. Может быть "Company" или "Personal". Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Это свойство доступно только для чтения.|
|манажементстате|[манажементстате](../resources/intune-devices-managementstate.md)|Состояние управления для устройства. Это свойство доступно только для чтения. Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Это свойство доступно только для чтения.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Это свойство доступно только для чтения.|
|чассистипе|[чассистипе](../resources/intune-devices-chassistype.md)|Тип корпуса устройства. Это свойство доступно только для чтения. Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Это свойство доступно только для чтения.|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Платформа устройства. Это свойство доступно только для чтения. Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Это свойство доступно только для чтения.|
|managementAgent|[манажементаженттипе](../resources/intune-shared-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Это свойство доступно только для чтения. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|osVersion|String|Версия операционной системы устройства. Это свойство доступно только для чтения.|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync. Это свойство доступно только для чтения.|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Это свойство доступно только для чтения.|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Это свойство доступно только для чтения.|
|аадрегистеред|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения.|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации устройства. Это свойство доступно только для чтения. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.|
|лостмодестате|[лостмодестате](../resources/intune-devices-lostmodestate.md)|Указывает, включен ли режим потерянных или отключенных. Это свойство доступно только для чтения. Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Это свойство доступно только для чтения.|
|emailAddress|String|Сообщения электронной почты пользователя, связанного с устройством. Это свойство доступно только для чтения.|
|Свойства azureactivedirectorydeviceid|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения.|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Это свойство доступно только для чтения. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемое имя категории устройств. Это свойство доступно только для чтения.|
|isSupervised|Boolean|Состояние контролируемого устройства. Это свойство доступно только для чтения.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Это свойство доступно только для чтения.|
|exchangeAccessState|[девицеманажементексчанжеакцессстате](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Это свойство доступно только для чтения. Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[девицеманажементексчанжеакцессстатереасон](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Это свойство доступно только для чтения. Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Это свойство доступно только для чтения.|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Это свойство доступно только для чтения.|
|isEncrypted|Boolean|Состояние шифрования устройства. Это свойство доступно только для чтения.|
|userPrincipalName|String|Имя участника пользователя устройства. Это свойство доступно только для чтения.|
|model|String|Модель устройства. Это свойство доступно только для чтения.|
|manufacturer|String|Производитель устройства. Это свойство доступно только для чтения.|
|imei|String|IMEI. Это свойство доступно только для чтения.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройства требованиям. Это свойство доступно только для чтения.|
|serialNumber|Строка|Серийный. Это свойство доступно только для чтения.|
|phoneNumber|String|Номер телефона устройства. Это свойство доступно только для чтения.|
|androidSecurityPatchLevel|String|Уровень обновления для системы безопасности Android. Это свойство доступно только для чтения.|
|userDisplayName|String|Отображаемое имя пользователя. Это свойство доступно только для чтения.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, поддерживающие клиент Конфигрмгр. Это свойство доступно только для чтения.|
|wiFiMacAddress|String|MAC Wi-Fi. Это свойство доступно только для чтения.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Это свойство доступно только для чтения.|
|subscriberCarrier|String|Перевозчик абонента. Это свойство доступно только для чтения.|
|meid|String|MEID. Это свойство доступно только для чтения.|
|totalStorageSpaceInBytes|Int64|Общий объем хранилища в байтах. Это свойство доступно только для чтения.|
|freeStorageSpaceInBytes|Int64|Свободное хранилище в байтах. Это свойство доступно только для чтения.|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем.|
|partnerReportedThreatState|[манажеддевицепартнеррепортедхеалсстате](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Это свойство доступно только для чтения. Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|ретиреафтердатетиме|DateTimeOffset|Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия. Это свойство доступно только для чтения.|
|усерслогжедон|Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)|Указывает последнего вошедшего в систему пользователя устройства. Это свойство доступно только для чтения.|
|префермдмоверграупполициапплиеддатетиме|DateTimeOffset|Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.  Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики. Только для чтения. Это свойство доступно только для чтения.|
|аутопилотенроллед|Boolean|Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот. Это свойство доступно только для чтения.|
|рекуиреусеренроллментаппровал|Boolean|Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя. Это свойство доступно только для чтения.|
|манажементцертификатикспиратиондате|DateTimeOffset|Дата окончания срока действия сертификата управления устройствами. Это свойство доступно только для чтения.|
|икЦид|String|Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты. Это свойство доступно только для чтения.|
|удид|String|Уникальный идентификатор устройства для устройств iOS и macOS. Это свойство доступно только для чтения.|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого экземпляра устройства.|
|виндовсактивемалварекаунт|Int32|Количество активных вредоносных программ для этого устройства Windows. Это свойство доступно только для чтения.|
|виндовсремедиатедмалварекаунт|Int32|Количество исправленных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения.|
|notes|String|Примечания к устройству, созданному ИТ ИТ Admin|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел или управляемых с помощью агентов ConfigMgr|
|есернетмакаддресс|String|MAC Ethernet. Это свойство доступно только для чтения.|
|фисикалмеморинбитес|Int64|Общий объем памяти в байтах. Это свойство доступно только для чтения.|
|процессорарчитектуре|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Архитектура процессора. Это свойство доступно только для чтения. Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|спеЦификатионверсион|String|Версия спецификации. Это свойство доступно только для чтения.|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Тип присоединения устройства. Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|скуфамили|String|Семейство SKU устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Все установленные на устройстве приложения|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Категория устройства|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Состояние защиты устройства.|
|users|Коллекция объектов [user](../resources/intune-shared-user.md)|Основные пользователи, связанные с управляемым устройством.|

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
    "operatingSystemProductType": 1024
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
  "skuFamily": "String"
}
```



