---
title: Тип ресурса macOSGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 96afbda75427f83ec213d4e764b6612a33363f4c
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266886"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса macOSGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом macOSGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

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
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
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
|iCloudBlockMail|Логический|Указывает, следует ли блокировать iCloud при синхронизации почты.|
|iCloudBlockAddressBook|Логический|Указывает, следует ли блокировать iCloud при синхронизации контактов.|
|iCloudBlockCalendar|Логический|Указывает, следует ли блокировать iCloud от синхронизации календарей.|
|iCloudBlockReminders|Логический|Указывает, следует ли блокировать iCloud при синхронизации напоминаний.|
|iCloudBlockBookmarks|Логический|Указывает, следует ли блокировать iCloud при синхронизации закладок.|
|iCloudBlockNotes|Логический|Указывает, следует ли блокировать iCloud при синхронизации заметок.|
|airDropBlocked|Boolean|Указывает, разрешить или не разрешить AirDrop.|
|passwordBlockModification|Логический|Указывает, следует ли разрешить изменение пароля.|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockAutoFill|Логический|Указывает, следует ли блокировать функцию AutoFill Passwords.|
|passwordBlockProximityRequests|Логический|Указывает, следует ли блокировать запрашивающие пароли с близлежащих устройств.|
|passwordBlockAirDropSharing|Логический|Указывает, следует ли блокировать совместное использование паролей с помощью функции паролей AirDrop.|
|softwareUpdatesEnforcedDelayInDays|Int32|Задает время, за которое будет отламывно обновление программного обеспечения для контролируемого устройства. Допустимые значения: от 0 до 90.|
|updateDelayPolicy|[macOSSoftwareUpdateDelayPolicy](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|Определяет, откладывать ли обновления ОС и/или приложений для macOS. Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.|
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
|multiplayerGamingBlocked|Логический|Да, предотвращает многопользовательские игры при использовании Game Center. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|
|wallpaperModificationBlocked|Логический|Да, не позволяет изменить обои. Доступно для устройств с macOS-версиями 10.13 и более поздней версии.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

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
  "wallpaperModificationBlocked": true
}
```




