---
title: Тип ресурса macOSGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3213c0f5afed6acbce9db3f52f2115e24af5adc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666767"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса macOSGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом macOSGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление macOSGeneralDeviceConfigurations](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-list.md)|Коллекция [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Получение macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-get.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Считывание свойств и связей объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Создание macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-create.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Удаление macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-delete.md)|None|Удаление экземпляра [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Обновление macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-update.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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
|passwordMaximumAttemptCount|Int32|Число разрешенных неудачных попыток ввода секретного кода на экране блокировки устройства. Допустимые значения от 2 до 11|
|passwordMinutesUntilFailedLoginReset|Int32|Количество минут до сброса имени входа после максимального числа неудачных попыток входа.|
|keychainBlockCloudSync|Логический|Указывает, заблокирована ли синхронизация цепочки ключей iCloud (macOS 10.12 и более поздних версий).|
|safariBlockAutofill|Boolean|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|cameraBlocked|Boolean|Указывает, следует ли запретить доступ к камере устройства.|
|iTunesBlockMusicService|Boolean|Указывает, следует ли заблокировать службу "Музыка" и вернуть приложение "Музыка" в классический режим.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли запретить Spotlight возвращать результаты поиска в Интернете.|
|keyboardBlockDictation|Boolean|Указывает, следует ли запретить пользователю использовать входные данные диктовки.|
|definitionLookupBlocked|Boolean|Указывает, следует ли блокировать поиск определения.|
|appleWatchBlockAutoUnlock|Логическое|Указывает, следует ли запретить пользователям разблокировать компьютер Mac с помощью Apple Watch.|
|iTunesBlockFileSharing|Логическое|Указывает, следует ли блокировать передачу файлов с помощью iTunes.|
|iCloudBlockDocumentSync|Boolean|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockMail|Логическое|Указывает, следует ли блокировать синхронизацию почты в iCloud.|
|iCloudBlockAddressBook|Логическое|Указывает, следует ли блокировать синхронизацию контактов в iCloud.|
|iCloudBlockCalendar|Логическое|Указывает, следует ли блокировать синхронизацию календарей в iCloud.|
|iCloudBlockReminders|Логическое|Указывает, следует ли блокировать синхронизацию напоминаний в iCloud.|
|iCloudBlockBookmarks|Логическое|Указывает, следует ли блокировать синхронизацию закладок в iCloud.|
|iCloudBlockNotes|Логическое|Указывает, следует ли блокировать синхронизацию заметок в iCloud.|
|airDropBlocked|Boolean|Указывает, следует ли разрешить AirDrop.|
|passwordBlockModification|Логическое|Указывает, следует ли разрешить изменение секретного кода.|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockAutoFill|Логическое|Указывает, следует ли блокировать функцию автозаполнения паролей.|
|passwordBlockProximityRequests|Логическое|Указывает, следует ли блокировать запрос паролей с ближайших устройств.|
|passwordBlockAirDropSharing|Логическое|Указывает, следует ли блокировать общий доступ к паролям с помощью функции паролей AirDrop.|
|softwareUpdatesEnforcedDelayInDays|Int32|Задает количество дней, в течение которых будет выполняться отладка обновления программного обеспечения для защищенного устройства. Допустимые значения: от 0 до 90.|
|updateDelayPolicy|[macOSSoftwareUpdateDelayPolicy](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|Определяет, следует ли отложить обновления ОС и (или) приложений для macOS. Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`, `unknownFutureValue`, `delayMajorOsUpdateVisibility`.|
|contentCachingBlocked|Логическое|Указывает, следует ли разрешить кэширование содержимого.|
|iCloudBlockPhotoLibrary|Boolean|Указывает, следует ли заблокировать медиатеку iCloud.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|classroomAppBlockRemoteScreenObservation|Boolean|Указывает, следует ли разрешить удаленное наблюдение за экранами в приложении Classroom. Требуется регистрация MDM через Apple School Manager или Apple Business Manager.|
|classroomAppForceUnpromptedScreenObservation|Boolean|Указывает, следует ли автоматически предоставлять преподавателю управляемого курса в приложении Classroom разрешение на просмотр экрана учащегося без запроса. Требуется регистрация MDM через Apple School Manager или Apple Business Manager.|
|classroomForceAutomaticallyJoinClasses|Логическое|Указывает, следует ли автоматически предоставлять разрешения на запросы преподавателя без запроса учащегося. Требуется регистрация MDM через Apple School Manager или Apple Business Manager.|
|classroomForceRequestPermissionToLeaveClasses|Логическое|Указывает, должен ли учащийся, зарегистрированный в неуправляемом курсе через Classroom, запрашивать разрешение у преподавателя при попытке покинуть курс. Требуется регистрация MDM через Apple School Manager или Apple Business Manager.|
|classroomForceUnpromptedAppAndDeviceLock|Логическое|Указывает, следует ли разрешить преподавателю блокировать приложения или устройство без запроса учащегося. Требуется регистрация MDM через Apple School Manager или Apple Business Manager.|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли запретить пользователю продолжать работу, запущенную на устройстве MacOS на другом устройстве iOS или MacOS (MacOS 10.15 или более поздней версии).|
|privacyAccessControls|[Коллекция macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)|Список элементов управления политикой предпочтений конфиденциальности. Эта коллекция может содержать не более 10 000 элементов.|
|addingGameCenterFriendsBlocked|Логическое|Да, пользователи не могут добавлять друзей в Game Center. Доступно для устройств под управлением macOS версии 10.13 и более поздних.|
|gameCenterBlocked|Boolean|Да отключает Game Center, а значок Game Center удаляется с начального экрана. Доступно для устройств под управлением macOS версии 10.13 и более поздних.|
|multiplayerGamingBlocked|Логическое|ЗНАЧЕНИЕ TRUE предотвращает многопользовательские игры при использовании Game Center. FALSE разрешает многопользовательские игры при использовании Game Center. Доступно для устройств под управлением macOS версии 10.13 и более поздних.|
|wallpaperModificationBlocked|Логическое|Значение TRUE предотвращает изменение фонового рисунка. Значение FALSE позволяет изменить фоновый рисунок. Доступно для устройств под управлением macOS версии 10.13 и более поздних.|
|eraseContentAndSettingsBlocked|Логическое|ЗНАЧЕНИЕ TRUE отключает параметр сброса на защищенных устройствах. False включает параметр сброса на защищенных устройствах. Доступно для устройств под управлением macOS версии 12.0 и более поздних.|
|softwareUpdateMajorOSDeferredInstallDelayInDays|Int32|Укажите количество дней (от 1 до 90) для задержки видимости основных обновлений программного обеспечения ОС. Доступно для устройств под управлением macOS версии 11.3 и более поздних. Допустимые значения: от 0 до 90.|
|softwareUpdateMinorOSDeferredInstallDelayInDays|Int32|Укажите количество дней (1–90) для задержки видимости дополнительных обновлений программного обеспечения ОС. Доступно для устройств под управлением macOS версии 11.3 и более поздних. Допустимые значения: от 0 до 90.|
|softwareUpdateNonOSDeferredInstallDelayInDays|Int32|Укажите количество дней (от 1 до 90) для задержки видимости обновлений программного обеспечения, отличных от ОС. Доступно для устройств под управлением macOS версии 11.3 и более поздних. Допустимые значения: от 0 до 90.|
|touchIdTimeoutInHours|Int32|Максимальное время, по истечении которого пользователь должен ввести пароль для разблокировки устройства вместо использования touch ID. Доступно для устройств под управлением macOS 12 и более поздних версий. Допустимые значения от 0 до 2147483647|
|iCloudPrivateRelayBlocked|Логическое|Частный ретранслятор iCloud — это служба iCloud+, которая запрещает сетям и серверам наблюдение за действиями пользователя в Интернете. Блокируя частный ретранслятор iCloud, Apple не шифрует трафик, исходящий с устройства. Доступно для устройств под управлением macOS 12 и более поздних версий.|
|iCloudDesktopAndDocumentsBlocked|Логическое|При значении TRUE синхронизация облачных рабочих столов и документов блокируется. При значении FALSE синхронизация облачного рабочего стола и документов разрешена. Доступно для устройств под управлением macOS 10.12.4 и более поздних версий.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 1024,
  "passwordMinutesUntilFailedLoginReset": 1024,
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
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "updateDelayPolicy": "String",
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
      "displayName": "String",
      "identifier": "String",
      "identifierType": "String",
      "codeRequirement": "String",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "String",
      "accessibility": "String",
      "addressBook": "String",
      "calendar": "String",
      "reminders": "String",
      "photos": "String",
      "mediaLibrary": "String",
      "fileProviderPresence": "String",
      "systemPolicyAllFiles": "String",
      "systemPolicySystemAdminFiles": "String",
      "systemPolicyDesktopFolder": "String",
      "systemPolicyDocumentsFolder": "String",
      "systemPolicyDownloadsFolder": "String",
      "systemPolicyNetworkVolumes": "String",
      "systemPolicyRemovableVolumes": "String",
      "postEvent": "String",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "String",
          "identifier": "String",
          "identifierType": "String",
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
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 1024,
  "touchIdTimeoutInHours": 1024,
  "iCloudPrivateRelayBlocked": true,
  "iCloudDesktopAndDocumentsBlocked": true
}
```




