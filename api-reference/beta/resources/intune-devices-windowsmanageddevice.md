---
title: Тип ресурса windowsManagedDevice
description: Устройства Windows, управляемые или предварительно зарегистрированные через Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1451a701fd50a8c277905b55f0f1e58c521fc88e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667406"
---
# <a name="windowsmanageddevice-resource-type"></a>Тип ресурса windowsManagedDevice

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройства Windows, управляемые или предварительно зарегистрированные через Intune


Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[Коллекция windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Список свойств и связей объектов [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Получение windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Чтение свойств и связей объекта [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Создание windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Создайте объект [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Удаление windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|Нет|Удаляет [объект windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[Обновление windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md);|Обновление свойств объекта [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Уникальный идентификатор пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Имя устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Подробные сведения об устройстве.  Включает такие сведения, как место в хранилище, производитель, серийный номер и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Владение устройством. Может быть "company" или "personal" Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Владение устройством. Может быть "company" или "personal" Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `company`, `personal`.|
|deviceActionResults|Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Список объектов deviceActionResult сложного типа.
 Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Состояние управления устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Время регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Дата и время последней успешной синхронизации устройства с Intune. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Тип корпуса устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Операционная система устройства. Windows, iOS и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|Платформа устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `desktop`, , `windowsRT``winMO6`, `nokia`, `windowsPhone`, `holoLens``macMDM``winCE``winEmbedded``mac``iPhone``iPod``android``iPad``androidForWork``unix``surfaceHub``iSocConsumer``androidEnterprise`, `chromeOS``windows10x``androidnGMS``linux`, , , `blackberry`, . `palm``unknown``cloudPC`|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Указывает, является ли устройство взломанным или рутованным. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Канал управления устройством. Intune, EAS и т. д. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `eas`, , `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient``configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf``googleCloudDevicePolicyController`, , `microsoft365ManagedMdm`, . `msSense``intuneAosp`|
|osVersion|String|Версия операционной системы устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|Указывает, активировано ли устройство в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Идентификатор устройства в Exchange ActiveSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Время активации устройства в Exchange ActivationSync. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Указывает, зарегистрировано ли устройство в Azure Active Directory. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|Тип регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, , `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin``windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsAzureADJoinUsingDeviceAuth``windowsCoManagement`, , `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, , `androidEnterpriseFullyManaged`. `androidEnterpriseCorporateWorkProfile`|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Указывает, включен или отключен режим пропажи. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `disabled`, `enabled`.|
|activationLockBypassCode|String|Код, позволяющий обойти блокировку активации на устройстве. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Адреса электронной почты пользователя, связанного с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Уникальный идентификатор устройства Azure Active Directory. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Состояние регистрации устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Отображаемое имя категории устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Состояние устройства в защищенном состоянии. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Время последнего подключения устройства к Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Состояние доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Причина состояния доступа к устройству в Exchange. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL-адрес, позволяющий установить сеанс удаленного помощника с устройством. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Проблемы, возникающие при создании сеансов удаленного помощника. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Состояние шифрования устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Имя участника-пользователя устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|Модель устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|manufacturer|String|Производитель устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия устройств. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|String|SerialNumber. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Номер телефона устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Уровень исправления для системы безопасности Android. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Отображаемое имя пользователя. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Функции, включенные клиентом ConfigrMgr. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Состояние подтверждения работоспособности устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Оператор подписчика. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Общее хранилище в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Свободное хранилище в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Автоматически созданный идентификатор устройства. Может быть заменен понятным именем. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
 Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Указывает время после автоматического прекращения использования устройства из-за запланированного действия. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|usersLoggedOn|[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)|Указывает последний вошед в систему пользователей устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Сообщает dateTime, где задано значение preferMdmOverGroupPolicy.  Если этот параметр задано, Intune MDM переопределит групповая политика параметров в случае конфликта. Только для чтения. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Логическое|Сообщает, зарегистрировано ли управляемое устройство с помощью автоматического пилотного развертывания. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Логическое|Сообщает, является ли управляемое устройство iOS регистрацией утверждения пользователя. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Сообщает дату окончания срока действия сертификата управления устройствами. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Iccid|String|Интегрированный идентификатор карты канала — это уникальный идентификационный номер SIM-карты. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|udid|String|Уникальный идентификатор устройства для устройств iOS и macOS. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|Идентификаторы roleScopeTagId|Коллекция строк|Список идентификаторов тегов области для данного экземпляра устройства. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Количество активных вредоносных программ для этого устройства Windows. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Число исправленных вредоносных программ для этого устройства Windows. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Заметки об устройстве, созданном ИТ Администратор унаследованным от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Состояние работоспособности клиента Configuration Manager, допустимое только для устройств, управляемых агентом MDM или ConfigMgr, унаследованным от [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Сведения о клиенте Configuration Manager, действительные только для устройств, управляемых, управляемых duel или три управляемых агентом ConfigMgr, унаследованных от [managedDevice](../resources/intune-devices-manageddevice.md)|
|EthernetMacAddress|String|Ethernet MAC. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|physicalMemoryInBytes|Int64|Общий объем памяти в байтах. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Архитектура процессора. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|specificationVersion|String|Версия спецификации. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Тип соединения устройства, унаследованный [от managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|skuFamily|String|Семейство номеров SKU устройства, унаследованных [от managedDevice](../resources/intune-devices-manageddevice.md)|
|skuNumber|Int32|Номер SKU устройства, см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo. Допустимые значения от 0 до 2147483647. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|Функции управления устройствами, унаследованные [от managedDevice](../resources/intune-devices-manageddevice.md). Возможные значения: `none`, `microsoftManagedDesktop`.|
|chromeOSDeviceInfo|[Коллекция chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md)|Список свойств устройства ChromeOS. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|enrollmentProfileName|String|Имя профиля регистрации, назначенного устройству. Значение по умолчанию — пустая строка, указывающая, что профиль регистрации не был задан. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|bootstrapTokenEscrowed|Логическое|Сообщает, имеет ли управляемое устройство токен начальной загрузки с депонированной загрузкой. Это применимо только к устройствам macOS. Если значение равно FALSE, то маркер начальной загрузки не депонируются. Если значение равно TRUE, устройство депонированное токен начальной загрузки с Intune. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceFirmwareConfigurationInterfaceManaged|Логическое|Указывает, управляется ли устройство DFCI. При значении TRUE устройство управляется DFCI. Если значение равно FALSE, устройство не управляется DFCI. Значение по умолчанию — FALSE. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Все приложения, установленные в настоящее время на устройстве Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-devices-devicecategory.md)|Категория устройства, наследуемая [от managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Состояние защиты устройства. Это свойство доступно только для чтения. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|users|Коллекция объектов [user](../resources/intune-devices-user.md)|Основные пользователи, связанные с управляемым устройством. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)|
|logCollectionRequests|[Коллекция deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Список запросов на сбор журналов, унаследованных от [managedDevice](../resources/intune-devices-manageddevice.md)|

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
    "subnetAddress": "String",
    "esimIdentifier": "String",
    "systemManagementBIOSVersion": "String",
    "tpmManufacturer": "String",
    "tpmVersion": "String",
    "wiredIPv4Addresses": [
      "String"
    ],
    "batteryLevelPercentage": "4.2",
    "residentUsersCount": 1024,
    "productName": "String",
    "deviceLicensingStatus": "String",
    "deviceLicensingLastErrorCode": 1024,
    "deviceLicensingLastErrorDescription": "String"
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
  "managementFeatures": "String",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "String",
      "value": "String",
      "valueType": "String",
      "updatable": true
    }
  ],
  "enrollmentProfileName": "String",
  "bootstrapTokenEscrowed": true,
  "deviceFirmwareConfigurationInterfaceManaged": true
}
```




