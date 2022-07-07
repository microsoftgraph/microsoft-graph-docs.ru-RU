---
title: Тип ресурса macOSDeviceFeaturesConfiguration
description: Профиль конфигурации функций устройства MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 841066482be31c904b363a3be98fb9e65d40eea6
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669100"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a>Тип ресурса macOSDeviceFeaturesConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации функций устройства MacOS.


Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов macOSDeviceFeaturesConfigurations](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|Коллекция [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Список свойств и связей объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Получение объекта macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Чтение свойств и связей объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Создание объекта macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Удаление объекта macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|Нет|Удаляет объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Обновление объекта macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|

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
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|airPrintDestinations|[Коллекция airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)|Массив принтеров AirPrint, который всегда должен отображаться. Эта коллекция может содержать не более 500 элементов. Наследуется [от appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|
|autoLaunchItems|[Коллекция macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)|Список приложений, файлов, папок и других элементов, запускаемых при входе пользователя в систему. Эта коллекция может содержать не более 500 элементов.|
|adminShowHostInfo|Логическое|Указывает, следует ли отображать сведения о узле администратора в окне входа.|
|loginWindowText|String|Пользовательский текст, отображаемый в окне входа.|
|authorizedUsersListHidden|Логическое|Указывает, следует ли отображать диалоговое окно имени и пароля или список пользователей в окне входа.|
|authorizedUsersListHideLocalUsers|Логическое|Следует ли отображать только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideMobileAccounts|Логическое|Следует ли скрывать мобильных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListIncludeNetworkUsers|Логическое|Следует ли отображать сетевых пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideAdminUsers|Логическое|Следует ли скрывать пользователей администратора в списке авторизованных пользователей в окне входа.|
|authorizedUsersListShowOtherManagedUsers|Логическое|Следует ли отображать других пользователей в списке авторизованных пользователей в окне входа.|
|shutDownDisabled|Логическое|Следует ли скрыть элемент кнопки "Завершить работу" в окне входа.|
|restartDisabled|Логическое|Следует ли скрыть элемент кнопки "Перезапустить" в окне входа.|
|sleepDisabled|Логическое|Следует ли скрывать пункт меню "Спящий режим" в окне входа.|
|consoleAccessDisabled|Логическое|Будет ли другой пользователь игнорировать использование специального `console` имени пользователя.|
|shutDownDisabledWhileLoggedIn|Логическое|Будет ли отключен пункт меню "Завершение работы" в окне входа во время входа пользователя.|
|restartDisabledWhileLoggedIn|Логическое|Будет ли пункт меню "Перезапустить" в окне входа отключен во время входа пользователя.|
|powerOffDisabledWhileLoggedIn|Логическое|Будет ли отключен пункт меню Power Off в окне входа во время входа пользователя.|
|logOutDisabledWhileLoggedIn|Логическое|Будет ли отключен пункт меню "Выход" в окне входа во время входа пользователя.|
|screenLockDisableImmediate|Логическое|Следует ли отключить функции немедленной блокировки экрана.|
|associatedDomains|Коллекция [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|НЕ РЕКОМЕНДУЕТСЯ: вместо него используйте appAssociatedDomains. Возвращает или задает список, который сопоставляет приложения со связанными доменами. Ключ должен соответствовать идентификатору приложения, а значение должно быть строкой в виде "service:domain", где домен является полным именем узла (например, webcredentials:example.com). Эта коллекция может содержать не более 500 элементов.|
|appAssociatedDomains|[Коллекция macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)|Возвращает или задает список, который сопоставляет приложения со связанными доменами. Идентификаторы приложений должны быть уникальными. Эта коллекция может содержать не более 500 элементов.|
|singleSignOnExtension|[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)|Возвращает или задает профиль расширения единого входа. Не рекомендуется: вместо этого используйте macOSSingleSignOnExtension.|
|macOSSingleSignOnExtension|[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)|Возвращает или задает профиль расширения единого входа.|
|contentCachingEnabled|Логический|Включает кэширование содержимого и предотвращает его отключение пользователем.|
|contentCachingType|[macOSContentCachingType](../resources/intune-deviceconfig-macoscontentcachingtype.md)|Определяет, какой тип содержимого разрешено кэшировать службой кэширования содержимого Apple. Возможные значения: `notConfigured`, `userContentOnly`, `sharedContentOnly`.|
|contentCachingMaxSizeBytes|Int64|Максимальное количество байтов дискового пространства, которое будет использоваться для кэша содержимого. Значение 0 (по умолчанию) указывает на неограниченное место на диске. |
|contentCachingDataPath|String|Путь к каталогу, используемому для хранения кэшированного содержимого. Значение должно быть (или о конце) /Library/Application Support/Apple/AssetCache/Data|
|contentCachingDisableConnectionSharing|Логическое|Отключает общий доступ к интернету.|
|contentCachingForceConnectionSharing|Логическое|Принудительное предоставление общего доступа к Интернету. ContentCachingDisableConnectionSharing переопределяет этот параметр.|
|contentCachingClientPolicy|[macOSContentCachingClientPolicy](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|Определяет метод, с помощью которого серверы кэширования содержимого будут прослушивать клиенты. Возможные значения: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.|
|contentCachingClientListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список кэшей содержимого настраиваемых диапазонов IP-адресов будет использоваться для прослушивания клиентов. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerPolicy|[macOSContentCachingPeerPolicy](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|Определяет метод, в котором содержимое кэширует одноранговый узел с другими кэшами. Возможные значения: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.|
|contentCachingPeerListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей содержимого диапазонов IP-адресов будет использоваться для прослушивания одноранговых кэшей. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerFilterRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список кэшей содержимого настраиваемых диапазонов IP-адресов будет использоваться для запроса содержимого из одноранговых кэшей. Эта коллекция может содержать не более 500 элементов.|
|contentCachingParentSelectionPolicy|[macOSContentCachingParentSelectionPolicy](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|Определяет метод, в котором серверы кэширования содержимого будут выбирать родительские элементы, если их несколько. Возможные значения: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.|
|contentCachingParents|Коллекция строк|Список IP-адресов, представляющих кэши родительского содержимого.|
|contentCachingLogClientIdentities|Логическое|Включает ведение журнала IP-адресов и портов клиентов, запрашивающего кэшированное содержимое.|
|contentCachingPublicRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список настраиваемых диапазонов IP-адресов, которые служба кэширования содержимого Apple должна использовать для сопоставления клиентов с кэшами содержимого. Эта коллекция может содержать не более 500 элементов.|
|contentCachingBlockDeletion|Логическое|Предотвращает очистку содержимого кэшами содержимого, чтобы освободить место на диске для других приложений.|
|contentCachingShowAlerts|Логическое|Отображение оповещений о кэшировании содержимого в виде системных уведомлений.|
|contentCachingKeep Транзакция|Логическое|Предотвращайте спящий режим устройства, если включено кэширование содержимого.|
|contentCachingPort|Int32|Задает порт, используемый для кэширования содержимого. Если значение равно 0, будет выбран случайный доступный порт. Допустимые значения от 0 до 65535|

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
|singleSignOnExtensionPkinitCertificate|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|PKINIT-сертификат для проверки подлинности с расширениями единого входа.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "String",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "String",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "String",
      "domains": [
        "String"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "String",
    "teamIdentifier": "String",
    "domains": [
      "String"
    ],
    "realm": "String",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "String",
        "value": "String"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "String",
    "domains": [
      "String"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "String",
    "credentialBundleIdAccessControlList": [
      "String"
    ],
    "domainRealms": [
      "String"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 1024,
    "passwordExpirationNotificationDays": 1024,
    "userPrincipalName": "String",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 1024,
    "passwordMinimumLength": 1024,
    "passwordMinimumAgeDays": 1024,
    "passwordRequirementsDescription": "String",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "String",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "String",
    "modeCredentialUsed": "String",
    "usernameLabelCustom": "String",
    "userSetupDelayed": true,
    "signInHelpText": "String",
    "kerberosAppsInBundleIdACLIncluded": true,
    "managedAppsInBundleIdACLIncluded": true,
    "credentialsCacheMonitored": true,
    "preferredKDCs": [
      "String"
    ],
    "tlsForLDAPRequired": true
  },
  "contentCachingEnabled": true,
  "contentCachingType": "String",
  "contentCachingMaxSizeBytes": 1024,
  "contentCachingDataPath": "String",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "String",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerPolicy": "String",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingParentSelectionPolicy": "String",
  "contentCachingParents": [
    "String"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 1024
}
```




