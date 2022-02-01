---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83ea52f359cb60fa795861be2be5901ec3a1ec27
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290919"
---
# <a name="update-macosdevicefeaturesconfiguration"></a>Обновление объекта macOSDeviceFeaturesConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

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
В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|airPrintDestinations|[коллекция airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)|Массив принтеров AirPrint, которые всегда должны быть показаны. Эта коллекция может содержать не более 500 элементов. Унаследованный от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|
|autoLaunchItems|[коллекция macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)|Список приложений, файлов, папок и других элементов, которые необходимо запустить при входе пользователя. Эта коллекция может содержать не более 500 элементов.|
|adminShowHostInfo|Логическое|Следует ли показывать сведения о хост-администраторе в окне входа.|
|loginWindowText|String|Пользовательский текст, отображаемый в окне входа.|
|authorizedUsersListHidden|Логический|Следует ли показывать диалоговое окно имени и пароля или список пользователей в окне входа.|
|authorizedUsersListHideLocalUsers|Логическое|Следует ли показывать только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideMobileAccounts|Логическое|Следует ли скрывать мобильных пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListIncludeNetworkUsers|Логическое|Следует ли показывать сетевых пользователей в списке авторизованных пользователей в окне входа.|
|authorizedUsersListHideAdminUsers|Логическое|Следует ли скрывать пользователей администратора в списке авторизованных пользователей в окне входа.|
|authorizedUsersListShowOtherManagedUsers|Логическое|Следует ли показывать других пользователей в списке авторизованного пользователя в окне входа.|
|shutDownDisabled|Логическое|Следует ли скрывать элемент кнопки Shut Down в окне входа.|
|restartDisabled|Логическое|Следует ли скрывать элемент кнопки Перезапуска в окне входа.|
|sleepDisabled|Логическое|Следует ли скрывать элемент меню Sleep в окне входа.|
|consoleAccessDisabled|Логическое|Будет ли другой пользователь игнорировать использование специального `console` имени пользователя.|
|shutDownDisabledWhileLoggedIn|Логическое|Будет ли отключен элемент меню Shut Down в окне входа во время входа пользователя.|
|restartDisabledWhileLoggedIn|Логическое|Будет ли элемент меню Перезапуска в окне входа отключен во время входа пользователя.|
|powerOffDisabledWhileLoggedIn|Логическое|Будет ли отключен элемент меню Power Off в окне входа во время входа пользователя.|
|logOutDisabledWhileLoggedIn|Логическое|Будет ли отключен элемент меню Log Out в окне входа во время входа пользователя.|
|screenLockDisableImmediate|Логическое|Следует ли отключить функции немедленной блокировки экрана.|
|associatedDomains|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|DEPRECATED: вместо этого используйте appAssociatedDomains. Получает или задает список, который сопополагает приложения с связанными доменами. Ключ должен соответствовать ID приложения, а значение должно быть строкой в виде "service:domain", где домен является полнокровным имям хост-сайта (например, webcredentials:example.com). Эта коллекция может содержать не более 500 элементов.|
|appAssociatedDomains|[коллекция macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)|Получает или задает список, который сопополагает приложения с связанными доменами. Идентификаторы приложений должны быть уникальными. Эта коллекция может содержать не более 500 элементов.|
|singleSignOnExtension|[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)|Получает или задает один профиль расширения для входов. Неуловимый: вместо этого используйте MacOSSingleSignOnExtension.|
|macOSSingleSignOnExtension|[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)|Получает или задает один профиль расширения для входов.|
|contentCachingEnabled|Логический|Включает кэшинг контента и предотвращает его отключение пользователем.|
|contentCachingType|[macOSContentCachingType](../resources/intune-deviceconfig-macoscontentcachingtype.md)|Определяет, какой тип контента разрешен кэшировали службой кэшинга контента Apple. Возможные значения: `notConfigured`, `userContentOnly`, `sharedContentOnly`.|
|contentCachingMaxSizeBytes|Int64|Максимальное количество bytes дискового пространства, которое будет использоваться для кэша контента. Значение 0 (по умолчанию) указывает на неограниченное пространство диска. |
|contentCachingDataPath|String|Путь к каталогу, используемый для хранения кэшного контента. Значение должно быть (или заканчивается) /Library/Application Support/Apple/AssetCache/Data|
|contentCachingDisableConnectionSharing|Логическое|Отключение общего доступа к Интернету.|
|contentCachingForceConnectionSharing|Логическое|Заставляет совместное использование подключения к Интернету. contentCachingDisableConnectionSharing переопределяет этот параметр.|
|contentCachingClientPolicy|[macOSContentCachingClientPolicy](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|Определяет метод, с помощью которого серверы кэшинга контента будут прослушивать клиентов. Возможные значения: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.|
|contentCachingClientListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания для клиентов. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerPolicy|[macOSContentCachingPeerPolicy](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|Определяет метод, в котором кэши контента соединяют с другими кэшами. Возможные значения: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.|
|contentCachingPeerListenRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания одноранговых кэшей. Эта коллекция может содержать не более 500 элементов.|
|contentCachingPeerFilterRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских кэшей контента диапазонов IP будет использовать для запроса контента из кэшей одноранговых. Эта коллекция может содержать не более 500 элементов.|
|contentCachingParentSelectionPolicy|[macOSContentCachingParentSelectionPolicy](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|Определяет метод, при котором серверы кэшинга контента будут выбирать родителей, если их несколько. Возможные значения: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.|
|contentCachingParents|Коллекция строк|Список IP-адресов, представляющих кэши родительского контента.|
|contentCachingLogClientIdentities|Логический|Включает ведение журнала IP-адресов и портов клиентов, запрашивает кэширование контента.|
|contentCachingPublicRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Список пользовательских диапазонов IP-адресов, которые служба кэшинга контента Apple должна использовать для совпадения клиентов с кэшами контента. Эта коллекция может содержать не более 500 элементов.|
|contentCachingBlockDeletion|Логическое|Предотвращает очистку содержимого от кэшей контента, чтобы освободить пространство диска для других приложений.|
|contentCachingShowAlerts|Логическое|Отображение оповещений кэшинга контента в качестве системных уведомлений.|
|contentCachingKeepAwake|Логическое|Запретить устройству спать, если включен кэшинг контента.|
|contentCachingPort|Int32|Задает порт, используемый для кэшинга контента. Если значение 0, будет выбран случайный доступный порт. Допустимые значения от 0 до 65535|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6089

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
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
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/",
    "modeCredentialUsed": "Mode Credential Used value",
    "usernameLabelCustom": "Username Label Custom value",
    "userSetupDelayed": true,
    "signInHelpText": "Sign In Help Text value",
    "kerberosAppsInBundleIdACLIncluded": true,
    "managedAppsInBundleIdACLIncluded": true,
    "credentialsCacheMonitored": true,
    "preferredKDCs": [
      "Preferred KDCs value"
    ],
    "tlsForLDAPRequired": true
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6261

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
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
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/",
    "modeCredentialUsed": "Mode Credential Used value",
    "usernameLabelCustom": "Username Label Custom value",
    "userSetupDelayed": true,
    "signInHelpText": "Sign In Help Text value",
    "kerberosAppsInBundleIdACLIncluded": true,
    "managedAppsInBundleIdACLIncluded": true,
    "credentialsCacheMonitored": true,
    "preferredKDCs": [
      "Preferred KDCs value"
    ],
    "tlsForLDAPRequired": true
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```




