---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ceeed458506fe0cd0609b2ffcc1ae9fb13958bc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791707"
---
# <a name="update-macosgeneraldeviceconfiguration"></a>Update macOSGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

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
В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Список, включенный в CompliantAppsList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|Коллекция String|Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.|
|passwordBlockSimple|Boolean|Блокировка простых паролей.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля.|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать пароль. Допустимые значения: от 0 до 4.|
|passwordMinimumLength|Int32|Минимальная длина паролей.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Период бездействия (в минутах), по истечении которого будет гаснуть экран.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Boolean|Определяет, нужно ли запрашивать ввод пароля.|
|passwordMaximumAttemptCount|Int32|Количество разрешенных неудачных попыток ввести пароль на экране блокировки устройства. Допустимые значения от 2 до 11|
|passwordMinutesUntilFailedLoginReset|Int32|Количество минут до сброса входа после максимального количества неудачных попыток входа.|
|keychainBlockCloudSync|Логический|Указывает, заблокирована ли синхронизация ключей iCloud (macOS 10.12 и более поздней).|
|safariBlockAutofill|Boolean|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|cameraBlocked|Boolean|Указывает, следует ли запретить доступ к камере устройства.|
|iTunesBlockMusicService|Boolean|Указывает, следует ли блокировать службу "Музыка" и перенаторять приложение Music в классический режим.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли блокировать Spotlight для возврата результатов поиска в Интернете.|
|keyboardBlockDictation|Boolean|Указывает, следует ли блокировать пользователю использование ввода диктанта.|
|definitionLookupBlocked|Boolean|Указывает, следует ли блокировать просмотр определения.|
|AppleWatchBlockAutoUnlock|Логический|Указывает, следует ли блокировать пользователям разблокировку mac с помощью Apple Watch.|
|iTunesBlockFileSharing|Логический|Указывает, следует ли блокировать перенос файлов с помощью iTunes.|
|iCloudBlockDocumentSync|Boolean|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockMail|Boolean|Указывает, следует ли блокировать iCloud при синхронизации почты.|
|iCloudBlockAddressBook|Логический|Указывает, следует ли блокировать iCloud при синхронизации контактов.|
|iCloudBlockCalendar|Логический|Указывает, следует ли блокировать iCloud от синхронизации календарей.|
|iCloudBlockReminders|Логический|Указывает, следует ли блокировать iCloud при синхронизации напоминаний.|
|iCloudBlockBookmarks|Логический|Указывает, следует ли блокировать iCloud при синхронизации закладок.|
|iCloudBlockNotes|Boolean|Указывает, следует ли блокировать iCloud при синхронизации заметок.|
|airDropBlocked|Boolean|Указывает, разрешить или не разрешить AirDrop.|
|passwordBlockModification|Boolean|Указывает, следует ли разрешить изменение пароля.|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockAutoFill|Boolean|Указывает, следует ли блокировать функцию AutoFill Passwords.|
|passwordBlockProximityRequests|Логический|Указывает, следует ли блокировать запрашивающие пароли с близлежащих устройств.|
|passwordBlockAirDropSharing|Boolean|Указывает, следует ли блокировать совместное использование паролей с помощью функции паролей AirDrop.|
|softwareUpdatesEnforcedDelayInDays|Int32|Задает время, за которое будет отламывно обновление программного обеспечения для контролируемого устройства. Допустимые значения: от 0 до 90.|
|updateDelayPolicy|[macOSSoftwareUpdateDelayPolicy](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|Определяет, откладывать ли обновления ОС и/или приложений для macOS. Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`, `unknownFutureValue`, `delayMajorOsUpdateVisibility`.|
|contentCachingBlocked|Логический|Указывает, следует ли разрешить кэшинг контента.|
|iCloudBlockPhotoLibrary|Boolean|Указывает, следует ли заблокировать медиатеку iCloud.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|classroomAppBlockRemoteScreenObservation|Boolean|Указывает, следует ли разрешить удаленное наблюдение экрана в приложении Classroom. Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.|
|classroomAppForceUnpromptedScreenObservation|Boolean|Указывает, следует ли автоматически давать преподавателю управляемого курса в приложении Classroom разрешение на просмотр экрана учащегося без запроса. Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.|
|classroomForceAutomaticallyJoinClasses|Логический|Указывает, следует ли автоматически давать разрешения на запросы преподавателя без запроса учащегося. Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.|
|classroomForceRequestPermissionToLeaveClasses|Логический|Указывает, потребуется ли учащемуся, зарегистрированным на неугодном курсе через Класс, запрашивать разрешения у преподавателя при попытке покинуть курс. Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.|
|classroomForceUnpromptedAppAndDeviceLock|Логический|Указывает, следует ли разрешить преподавателю заблокировать приложения или устройство без запроса учащегося. Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли блокировать пользователю продолжение работы, которую они начали на устройстве MacOS на другом устройстве iOS или MacOS (MacOS 10.15 или более поздней).|
|privacyAccessControls|[коллекция macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)|Список элементов управления политиками конфиденциальности. Эта коллекция может содержать не более 10 000 элементов.|
|addingGameCenterFriendsBlocked|Логический|Да, не позволяет пользователям добавлять друзей в Game Center. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|
|gameCenterBlocked|Boolean|Да, отключает центр игры, и значок Центра игры удаляется с домашнего экрана. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|
|multiplayerGamingBlocked|Логический|TRUE предотвращает многопользовательские игры при использовании Game Center. FALSE позволяет многопользовательские игры при использовании Game Center. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|
|wallpaperModificationBlocked|Boolean|TRUE не позволяет изменить обои. FALSE позволяет изменить обои. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|
|eraseContentAndSettingsBlocked|Логический|TRUE отключает параметр сброса на контролируемых устройствах. FALSE включает параметр сброса на контролируемых устройствах. Доступно для устройств с macOS-версиями 12.0 и более поздней версии.|
|softwareUpdateMajorOSDeferredInstallDelayInDays|Int32|Укажите количество дней (1-90) для задержки видимости основных обновлений программного обеспечения ОС. Доступно для устройств с macOS-версиями 11.3 и более поздней версии. Допустимые значения: от 0 до 90.|
|softwareUpdateMinorOSDeferredInstallDelayInDays|Int32|Укажите количество дней (1-90) для задержки видимости незначительных обновлений программного обеспечения ОС. Доступно для устройств с macOS-версиями 11.3 и более поздней версии. Допустимые значения: от 0 до 90.|
|softwareUpdateNonOSDeferredInstallDelayInDays|Int32|Укажите количество дней (1-90) для задержки видимости обновлений программного обеспечения без ОС. Доступно для устройств с macOS-версиями 11.3 и более поздней версии. Допустимые значения: от 0 до 90.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4900

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ],
  "addingGameCenterFriendsBlocked": true,
  "gameCenterBlocked": true,
  "multiplayerGamingBlocked": true,
  "wallpaperModificationBlocked": true,
  "eraseContentAndSettingsBlocked": true,
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5072

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ],
  "addingGameCenterFriendsBlocked": true,
  "gameCenterBlocked": true,
  "multiplayerGamingBlocked": true,
  "wallpaperModificationBlocked": true,
  "eraseContentAndSettingsBlocked": true,
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13
}
```



