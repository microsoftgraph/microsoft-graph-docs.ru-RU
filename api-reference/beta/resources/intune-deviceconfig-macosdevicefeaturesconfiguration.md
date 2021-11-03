---
title: Тип ресурса macOSDeviceFeaturesConfiguration
description: Профиль конфигурации функций устройства MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ed5280c7f3b1274e73403935e433fb1d5f3ce0b
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684060"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a>Тип ресурса macOSDeviceFeaturesConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|airPrintDestinations|[коллекция airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)|Массив принтеров AirPrint, которые всегда должны быть показаны. Эта коллекция может содержать не более 500 элементов. Унаследованный от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|
|autoLaunchItems|[коллекция macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)|Список приложений, файлов, папок и других элементов, которые необходимо запустить при входе пользователя. Эта коллекция может содержать не более 500 элементов.|
|adminShowHostInfo|Логический|Следует ли показывать сведения о хост-администраторе в окне входа.|
|loginWindowText|String|Пользовательский текст, отображаемый в окне входа.|
|authorizedUsersListHidden|Логический|Следует ли показывать диалоговое окно имени и пароля или список пользователей в окне входа.|
|authorizedUsersListHideLocalUsers|Логический|Следует ли показывать только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideMobileAccounts|Логический|Следует ли скрывать мобильных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListIncludeNetworkUsers|Логический|Следует ли показывать сетевых пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideAdminUsers|Логический|Следует ли скрывать пользователей администратора в списке авторизованных пользователей в окне входа.|
|authorizedUsersListShowOtherManagedUsers|Логический|Следует ли показывать других пользователей в списке авторизованного пользователя в окне входа.|
|shutDownDisabled|Логический|Следует ли скрывать элемент кнопки Shut Down в окне входа.|
|restartDisabled|Логический|Следует ли скрывать элемент кнопки Перезапуска в окне входа.|
|sleepDisabled|Логический|Следует ли скрывать элемент меню Sleep в окне входа.|
|consoleAccessDisabled|Логический|Будет ли другой пользователь игнорировать использование `console` специального имени пользователя.|
|shutDownDisabledWhileLoggedIn|Логический|Будет ли отключен элемент меню Shut Down в окне входа во время входа пользователя.|
|restartDisabledWhileLoggedIn|Логический|Будет ли элемент меню Перезапуска в окне входа отключен во время входа пользователя.|
|powerOffDisabledWhileLoggedIn|Логический|Будет ли отключен элемент меню Power Off в окне входа во время входа пользователя.|
|logOutDisabledWhileLoggedIn|Логический|Будет ли отключен элемент меню Log Out в окне входа во время входа пользователя.|
|screenLockDisableImmediate|Логический|Следует ли отключить функции немедленной блокировки экрана.|
|associatedDomains|Коллекция [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|DEPRECATED: вместо этого используйте appAssociatedDomains. Получает или задает список, который сопополагает приложения с связанными доменами. Ключ должен соответствовать ID приложения, а значение должно быть строкой в виде "service:domain", где домен является полнокровным имям хост-сайта (например, webcredentials:example.com). Эта коллекция может содержать не более 500 элементов.|
|appAssociatedDomains|[коллекция macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)|Получает или задает список, который сопополагает приложения с связанными доменами. Идентификаторы приложений должны быть уникальными. Эта коллекция может содержать не более 500 элементов.|
|singleSignOnExtension|[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)|Получает или задает один профиль расширения для входов. Неуловимый: вместо этого используйте MacOSSingleSignOnExtension.|
|macOSSingleSignOnExtension|[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)|Получает или задает один профиль расширения для входов.|
|contentCachingEnabled|Логический|Включает кэшинг контента и предотвращает его отключение пользователем.|
|contentCachingType|[macOSContentCachingType](../resources/intune-deviceconfig-macoscontentcachingtype.md)|Определяет, какой тип контента разрешен кэшировали службой кэшинга контента Apple. Возможные значения: `notConfigured`, `userContentOnly`, `sharedContentOnly`.|
|contentCachingMaxSizeBytes|Int32|Максимальное количество bytes дискового пространства, которое будет использоваться для кэша контента. Значение 0 (по умолчанию) указывает на неограниченное пространство диска. |
|contentCachingDataPath|String|Путь к каталогу, используемый для хранения кэшного контента. Значение должно быть (или заканчивается) /Library/Application Support/Apple/AssetCache/Data|
|contentCachingDisableConnectionSharing|Логический|Отключение общего доступа к Интернету.|
|contentCachingForceConnectionSharing|Логический|Заставляет совместное использование подключения к Интернету. contentCachingDisableConnectionSharing переопределяет этот параметр.|
|contentCachingClientPolicy|[macOSContentCachingClientPolicy](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|Определяет метод, с помощью которого серверы кэшинга контента будут прослушивать клиентов. Возможные значения: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.|
|contentCachingClientListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания для клиентов. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerPolicy|[macOSContentCachingPeerPolicy](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|Определяет метод, в котором кэши контента соединяют с другими кэшами. Возможные значения: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.|
|contentCachingPeerListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания одноранговых кэшей. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerFilterRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для запроса контента из кэшей одноранговых. Эта коллекция может содержать не более 500 элементов.|
|contentCachingParentSelectionPolicy|[macOSContentCachingParentSelectionPolicy](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|Определяет метод, при котором серверы кэшинга контента будут выбирать родителей, если их несколько. Возможные значения: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.|
|contentCachingParents|Коллекция строк|Список IP-адресов, представляющих кэши родительского контента.|
|contentCachingLogClientIdentities|Логический|Включает ведение журнала IP-адресов и портов клиентов, запрашивает кэширование контента.|
|contentCachingPublicRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских диапазонов IP-адресов, которые служба кэшинга контента Apple должна использовать для совпадения клиентов с кэшами контента. Эта коллекция может содержать не более 500 элементов.|
|contentCachingBlockDeletion|Логический|Предотвращает очистку содержимого от кэшей контента, чтобы освободить пространство диска для других приложений.|
|contentCachingShowAlerts|Логический|Отображение оповещений кэшинга контента в качестве системных уведомлений.|
|contentCachingKeepAwake|Логический|Запретить устройству спать, если включен кэшинг контента.|
|contentCachingPort|Int32|Задает порт, используемый для кэшинга контента. Если значение 0, будет выбран случайный доступный порт. Допустимые значения от 0 до 65535|

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
|singleSignOnExtensionPkinitCertificate|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Сертификат PKINIT для проверки подлинности с одними расширениями для регистрации.|

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
    "usernameLableCustom": "String",
    "usernameLabelCustom": "String",
    "userSetupDelayed": true,
    "signInHelpText": "String",
    "kerberosAppsInBundleIdACLIncluded": true,
    "managedAppsInBundleIdACLIncluded": true,
    "credentialsCacheMonitored": true,
    "singleSignOnExtensionPreferredKDCs": [
      "String"
    ],
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



