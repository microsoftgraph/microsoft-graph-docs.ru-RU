---
title: Тип ресурса macOSGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом macOSGeneralDeviceConfiguration.
ms.openlocfilehash: 1b46ca91e5a9648b8fa63d3d0a8b565275921c52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080746"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса macOSGeneralDeviceConfiguration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|описание|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Список, включенный в CompliantAppsList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|Коллекция String|Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.|
|passwordBlockSimple|Boolean|Блокировка простых паролей.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля.|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать пароль. Допустимые значения: от 0 до 4.|
|passwordMinimumLength|Int32|Минимальная длина паролей.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Период бездействия (в минутах), по истечении которого гаснет экран.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Boolean|Указывает, обязательно ли использовать пароль.|
|keychainBlockCloudSync|Логический|Указывает, является ли iCloud ключей синхронизации заблокированных (macOS 10.12 и более поздних версий).|
|airPrintBlocked|Логический|Указывает, является ли AirPrint заблокированных (macOS 10.12 и более поздних версий).|
|airPrintForceTrustedTLS|Логический|Указывает, являются ли доверенные сертификаты для печати обмена данными TLS (macOS 10.13 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логический|Указывает, заблокирован ли обнаружения iBeacon AirPrint принтеров. Это позволяет предотвратить ложных маяки AirPrint Bluetooth от фишинга для сетевого трафика (macOS 10.3 и более поздних версий).|
|safariBlockAutofill|Логический|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|cameraBlocked|Логический|Указывает, следует ли запретить доступ к камере устройства.|
|iTunesBlockMusicService|Логический|Указывает, следует ли блокировать службы музыки и вернуться музыки приложения в классическом режиме.|
|spotlightBlockInternetResults|Логический|Указывает, следует ли запретить возвращение результатов из и поиск в Интернете в центре внимания.|
|keyboardBlockDictation|Логический|Указывает, следует ли пользователь с помощью диктовки входные данные.|
|definitionLookupBlocked|Логический|Указывает, следует ли блокировать определение подстановки.|
|appleWatchBlockAutoUnlock|Логический|Указывает, является ли или чтобы запретить пользователям разблокирование их Mac с Apple Watch.|
|iTunesBlockFileSharing|Логический|Указывает ли для блокировки файлов, из которых передаются с помощью iTunes.|
|iCloudBlockDocumentSync|Логический|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockMail|Логический|Указывает, следует ли блокировать iCloud синхронизацию почты.|
|iCloudBlockAddressBook|Логический|Указывает, следует ли блокировать iCloud синхронизацию контактов.|
|iCloudBlockCalendar|Логический|Указывает, следует ли блокировать iCloud из списка синхронизации календарей.|
|iCloudBlockReminders|Логический|Указывает, следует ли блокировать iCloud синхронизацию напоминания.|
|iCloudBlockBookmarks|Логический|Указывает, следует ли блокировать iCloud синхронизацию закладки.|
|iCloudBlockNotes|Логический|Указывает, следует ли блокировать iCloud синхронизацию заметки.|
|airDropBlocked|Логический|Указывает, следует ли разрешить AirDrop.|
|passwordBlockModification|Логический|Указывает, следует ли разрешить изменения секретный код.|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
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
  "passwordBlockFingerprintUnlock": true
}
```





