# <a name="manageddevice-resource-type"></a>Тип ресурса managedDevice

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Устройства, которые управляются или предварительно регистрируются с помощью Intune
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedDevice](../api/intune_devices_manageddevice_list.md)|Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)|Перечисление свойств и связей объектов [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Получение объекта managedDevice](../api/intune_devices_manageddevice_get.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Чтение свойств и связей объекта [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Создание объекта managedDevice](../api/intune_devices_manageddevice_create.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Создание объекта [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Удаление объекта managedDevice](../api/intune_devices_manageddevice_delete.md)|Нет|Удаление объекта [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Обновление объекта managedDevice](../api/intune_devices_manageddevice_update.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Обновление свойств объекта [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Действие retire](../api/intune_devices_manageddevice_retire.md)|Нет|Прекращение использования устройства|
|[Действие wipe](../api/intune_devices_manageddevice_wipe.md)|Нет|Очистка устройства|
|[Действие resetPasscode](../api/intune_devices_manageddevice_resetpasscode.md)|Нет|Сброс секретного кода|
|[Действие remoteLock](../api/intune_devices_manageddevice_remotelock.md)|Нет|Удаленная блокировка|
|[Действие requestRemoteAssistance](../api/intune_devices_manageddevice_requestremoteassistance.md)|Нет|Запрос удаленной помощи|
|[Действие disableLostMode](../api/intune_devices_manageddevice_disablelostmode.md)|Нет|Отключение режима пропажи устройства|
|[Действие locateDevice](../api/intune_devices_manageddevice_locatedevice.md)|Нет|Поиск устройства|
|[Действие bypassActivationLock](../api/intune_devices_manageddevice_bypassactivationlock.md)|Нет|Обход блокировки активации|
|[Действие rebootNow](../api/intune_devices_manageddevice_rebootnow.md)|Нет|Перезагрузка устройства|
|[Действие shutDown](../api/intune_devices_manageddevice_shutdown.md)|Нет|Завершение работы устройства|
|[Действие recoverPasscode](../api/intune_devices_manageddevice_recoverpasscode.md)|Нет|Восстановление секретного кода|
|[Действие cleanWindowsDevice](../api/intune_devices_manageddevice_cleanwindowsdevice.md)|Нет|Очистка устройства с Windows|
|[Действие logoutSharedAppleDeviceActiveUser](../api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md)|Нет|Выход от имени активного пользователя общего устройства Apple|
|[Действие deleteUserFromSharedAppleDevice](../api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md)|Нет|Удаление пользователя с общего устройства Apple|
|[Действие syncDevice](../api/intune_devices_manageddevice_syncdevice.md)|Нет|Н/Д|
|[Действие windowsDefenderScan](../api/intune_devices_manageddevice_windowsdefenderscan.md)|Нет|Н/Д|
|[Действие windowsDefenderUpdateSignatures](../api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md)|Нет|Н/Д|
|[Действие updateWindowsDeviceAccount](../api/intune_devices_manageddevice_updatewindowsdeviceaccount.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства.|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством.|
|deviceName|String|Название устройства|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune_devices_manageddeviceownertype.md)|Владение устройством. Может быть "компания" или "личное". Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|Список объектов deviceActionResult сложного типа.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д.|
|complianceState|[complianceState](../resources/intune_devices_compliancestate.md)|Состояние соответствия устройства требованиям. Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным.|
|managementAgent|[managementAgentType](../resources/intune_devices_managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|osVersion|String|Версия операционной системы устройства.|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync.|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync.|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync.|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune_shared_deviceenrollmenttype.md)|Тип регистрации устройства. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве.|
|emailAddress|String|Адреса электронной почты пользователя, связанного с устройством|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune_devices_deviceregistrationstate.md)|Состояние регистрации устройства. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемое имя категории устройства|
|isSupervised|Boolean|Состояние защиты устройства|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange.|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|Состояние доступа устройств в Exchange. Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника.|
|isEncrypted|Boolean|Состояние шифрования устройства|
|userPrincipalName|String|Имя участника-пользователя устройства|
|model|String|Модель устройства|
|manufacturer|String|Производитель устройства|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройства требованиям|
|serialNumber|String|SerialNumber|
|phoneNumber|String|Номер телефона устройства|
|androidSecurityPatchLevel|String|Уровень обновления для системы безопасности Android|
|userDisplayName|String|Отображаемое имя пользователя|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|Включенные функции клиента Configuration Manager|
|wiFiMacAddress|String|MAC-адрес сети Wi-Fi|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune_devices_devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства.|
|subscriberCarrier|String|Оператор сотовой связи, используемый абонентом|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|Общий объем хранилища в байтах|
|freeStorageSpaceInBytes|Int64|Свободный объем хранилища в байтах|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве). Только для чтения. Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune_shared_devicecategory.md)|Категория устройства|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
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
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
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
    "windowsUpdateForBusiness": true
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
  "partnerReportedThreatState": "String"
}
```








