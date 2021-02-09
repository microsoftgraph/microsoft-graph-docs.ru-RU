---
title: Создание windowsManagedDevice
description: Создание объекта windowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d16e4f661bf72ac4a3212f2caae1dd935bd61b51
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161189"
---
# <a name="create-windowsmanageddevice"></a>Создание windowsManagedDevice

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/comanagedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта windowsManagedDevice в JSON.

В следующей таблице показаны свойства, необходимые при создании объекта windowsManagedDevice.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|deviceName|String|Имя устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Подробные сведения об устройстве.  Включает такие сведения, как место в хранилище, изготовитель, серийный номер и т. д. Это свойство находится только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Владение устройством. Может иметь "company" или "personal". Наследуется от [managedDevice.](../resources/intune-shared-manageddevice.md) Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Владение устройством. Может быть "company" или "personal". Наследуется от [managedDevice.](../resources/intune-shared-manageddevice.md) Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Состояние управления устройством. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Тип корпусов устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Это свойство находится только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Платформа устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` , `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Это свойство находится только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|osVersion|String|Версия операционной системы устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|aadRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Указывает, включен ли режим потери. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|emailAddress|String|Электронная почта пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемая имя категории устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|isSupervised|Boolean|Состояние устройства под контролем. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|isEncrypted|Boolean|Состояние шифрования устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|userPrincipalName|String|Имя пользователя устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|model|String|Модель устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|manufacturer|String|Производитель устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|imei|String|IMEI. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройств требованиям. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|serialNumber|String|SerialNumber. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|phoneNumber|String|Номер телефона устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|androidSecurityPatchLevel|String|Уровень исправлений для системы безопасности Android. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|userDisplayName|String|Отображаемая имя пользователя. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, включенные клиентом ConfigrMgr. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|subscriberCarrier|String|Оператор подписчика. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|meid|String|MEID. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Общее хранилище в ветвях. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Бесплатное хранилище в вайтах. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Указывает время после автоматического выхода устройства из-за запланированного действия. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|usersLoggedOn|[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)|Указывает последних во время входа пользователей устройства. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Сообщает dateTime, задав параметр preferMdmOverGroupPolicy.  Если этот параметр задан, параметры MDM Intune переопредят параметры групповой политики в случае конфликта. Только для чтения. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|autopilotEnrolled|Boolean|Сообщает, зарегистрировать ли управляемое устройство с помощью автоматического пилотного проекта. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|Сообщает, является ли управляемое устройство iOS зарегистрированным пользователем. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Сообщает дату окончания срока действия сертификата управления устройствами. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|iccid|String|Интегрированный идентификатор схемной карты — это уникальный идентификационный номер SIM-карты. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|udid|String|Уникальный идентификатор устройства для устройств с iOS и macOS. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|roleScopeTagIds|Коллекция String|Список ИД тегов области для этого экземпляра устройства. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Количество активных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Количество исправленных вредоносных программ для этого устройства с Windows. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|notes|String|Примечания на устройстве, созданном ИТ-администратором. [Наследуется от managedDevice](../resources/intune-shared-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние состояния клиента Configuration Manager, действительное только для устройств, управляемых агентом MDM/ConfigMgr. Наследуется от [managedDevice](../resources/intune-shared-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Сведения о клиенте configuration manager, действительные только для устройств, управляемых, управляемых duel или триуправленных агентом ConfigMgr. Наследуется от [managedDevice](../resources/intune-shared-manageddevice.md)|
|ethernetMacAddress|String|Ethernet MAC. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|physicalMemoryInBytes|Int64|Общий объем памяти в ветвях. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Архитектура процессора. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md). Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|specificationVersion|String|Версия спецификации. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Тип следования устройства [Наследуется от managedDevice.](../resources/intune-shared-manageddevice.md) Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|skuFamily|String|Семейство SKU устройства Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|skuNumber|Int32|Номер SKU устройства, см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo . Допустимые значения: от 0 до 2 147 483 647. Это свойство доступно только для чтения. Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|Функции управления устройствами. [Наследуется от managedDevice.](../resources/intune-shared-manageddevice.md) Возможные значения: `none`, `microsoftManagedDesktop`.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 8115

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
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
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8164

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
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
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```




