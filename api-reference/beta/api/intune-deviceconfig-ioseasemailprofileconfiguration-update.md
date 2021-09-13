---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27b57388e3dc35c6c5a9d4fe8c69149abd9796de
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59116992"
---
# <a name="update-ioseasemailprofileconfiguration"></a>Обновление iosEasEmailProfileConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)

В следующей таблице показаны свойства, необходимые при создании [iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве. Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md);|Имя поля AAD, которое будет использоваться для получения имени пользователя для профиля электронной почты. Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);|Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве. Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `fullDomainName`, `netBiosDomainName`.|
|customDomainName|String|Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве. Унаследовано от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|имя учетной записи|String|Имя учетной записи.|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Метод проверки подлинности для этого профиля электронной почты. Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|blockMovingMessagesToOtherEmailAccounts|Логическое|Указывает, следует ли блокировать перемещение сообщений на другие учетные записи электронной почты.|
|blockSendingEmailFromThirdPartyApps|Логический|Указывает, следует ли блокировать отправку электронной почты из сторонних приложений.|
|blockSyncingRecentlyUsedEmailAddresses|Логический|Указывает, следует ли блокировать синхронизацию недавно используемых адресов электронной почты, например , при записи новой электронной почты.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность времени электронной почты должна быть синхронизирована. . Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве. Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|easServices|[easServices](../resources/intune-deviceconfig-easservices.md)|Exchange синхронизировать данные. Возможные значения: `none` `calendars` , , , `contacts` , `email` `notes` `reminders` .|
|easServicesUserOverrideEnabled|Логическое|Разрешить пользователям изменять параметры синхронизации.|
|hostName|String|Exchange( URL-адрес), к которое подключается приложение почты.|
|requireSmime|Логическое|Указывает, следует ли использовать сертификат S/MIME.|
|smimeEnablePerMessageSwitch|Логическое|Указывает, следует ли разрешить незашифрованные сообщения электронной почты.|
|smimeEncryptByDefaultEnabled|Логический|Если установлено значение true S/MIME- шифрование включено по умолчанию.|
|smimeSigningEnabled|Логический|Если для этой учетной записи включено правильное подписание S/MIME|
|smimeSigningUserOverrideEnabled|Логическое|Если установлено, что это так, пользователь может отключить вход или отключение подписи S/MIME.|
|smimeEncryptByDefaultUserOverrideEnabled|Логическое|Если установлено значение true, пользователь может настроить шифрование по умолчанию.|
|smimeSigningCertificateUserOverrideEnabled|Логический|Если установлено, что это так, пользователь может выбрать идентификатор подписи.|
|smimeEncryptionCertificateUserOverrideEnabled|Логический|Если установлено верно, пользователь может выбрать идентификатор шифрования S/MIME. |
|requireSsl|Логическое|Указывает, следует ли использовать SSL.|
|useOAuth|Логическое|Указывает, следует ли подключению использовать OAuth для проверки подлинности.|
|signingCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Подписание типа сертификата для этого профиля электронной почты. Возможные значения: `none`, `certificate`, `derivedCredential`.|
|encryptionCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Тип сертификата шифрования для этого профиля электронной почты. Возможные значения: `none`, `certificate`, `derivedCredential`.|
|perAppVPNProfileId|String|ID профиля политики VPN Per-App для доступа к электронным письмам от родного клиента почты|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2187

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2359

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```



