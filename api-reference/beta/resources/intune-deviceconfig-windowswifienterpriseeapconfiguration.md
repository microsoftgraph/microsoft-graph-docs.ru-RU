---
title: тип ресурса windowsWifiEnterpriseEAPConfiguration
description: Эта сущность содержит описания объявленных методов, свойств и связей, открытых CSP Wifi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 157a423f34fb9e7efa68c7c0a67d42b1f127e1b9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696611"
---
# <a name="windowswifienterpriseeapconfiguration-resource-type"></a>тип ресурса windowsWifiEnterpriseEAPConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит описания объявленных методов, свойств и связей, открытых CSP Wifi.


Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsWifiEnterpriseEAPConfigurations](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-list.md)|[коллекция windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Список свойств и связей [объектов WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|
|[Получить windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-get.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Чтение свойств и связей [объекта WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|
|[Создание windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-create.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Создайте [новый объект WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|
|[Удаление windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-delete.md)|Нет|Удаляет [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).|
|[Обновление windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-update.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Обновление свойств объекта [WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|

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
|preSharedKey|String|Это предварительный общий ключ для сети персональных Wi-Fi WPA. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Укажите тип безопасности Wi-Fi. Унаследовано от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Укажите тип ограничения дозы подключения для подключения Wi-Fi. Унаследовано от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Возможные значения: `unrestricted`, `fixed`, `variable`.|
|ssid|String|Укажите SSID подключения Wi-Fi. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkName|String|Укажите имя конфигурации сети. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectAutomatically|Логический|Укажите, должно ли подключение Wi-Fi подключаться автоматически при диапазоне. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectToPreferredNetwork|Логический|Укажите, должно ли подключение Wi-Fi подключаться к более предпочтительным сетям при уже подключении к этой.  Требуется, чтобы ConnectAutomatically был правдивым. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Логический|Укажите, следует ли подключать подключение к Wi-Fi автоматически, даже если SSID не транслируется. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Укажите параметр прокси для Wi-Fi конфигурации, унаследованной от [windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md) Возможные значения: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Укажите IP-адрес прокси-сервера. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyManualPort|Int32|Укажите порт для прокси-сервера. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|Укажите URL-адрес сценария конфигурации прокси-сервера. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|forceFIPSCompliance|Логический|Укажите, следует ли принудительно принудить к соблюдению FIPS. Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|Укажите сетевой единый знак по типу. Возможные значения: `disabled`, `prelogon`, `postlogon`.|
|maximumAuthenticationTimeoutInSeconds|Int32|Укажите максимальное время проверки подлинности (в секундах).  Допустимый диапазон: 1-120|
|userBasedVirtualLan|Логический|Указывает, следует ли изменять виртуальный LAN-интерфейс, используемый устройством на основе учетных данных пользователя. Нельзя использовать, если для NetworkSingleSignOnType установлено отключение.|
|promptForAdditionalAuthenticationCredentials|Логический|Укажите, должно ли подключение Wi-Fi подсказать дополнительные учетные данные проверки подлинности.|
|enablePairwiseMasterKeyCaching|Логический|Укажите, должно ли подключение Wi-Fi включить кэшинг ключей в парной области.|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|Укажите максимальное время кэша мастер-ключа парной стрелки (в минутах).  Допустимый диапазон: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|Укажите максимальное количество ключей в кэше с парной стрелкой.  Допустимый диапазон: 1-255|
|enablePreAuthentication|Логический|Укажите, должна ли быть включена предварительная проверка подлинности.|
|maximumPreAuthenticationAttempts|Int32|Укажите максимальные попытки предварительной проверки подлинности.  Допустимый диапазон: 1-16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication Protocol (EAP). Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|trustedServerCertificateNames|Коллекция строк|Укажите имена доверенных сертификатов сервера.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Укажите метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Укажите внутренний протокол проверки подлинности для TTLS EAP. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Укажите строку для замены имен пользователей для конфиденциальности при использовании EAP TTLS или PEAP.|
|requireCryptographicBinding|Логический|Укажите, следует ли включить криптографическую привязку при выборе типа EAP в качестве PEAP.|
|performServerValidation|Логический|Укажите, следует ли включить проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.|
|disableUserPromptForServerValidation|Логический|Укажите, следует ли запретить пользователю авторизировать новые серверы для доверенных органов сертификации при выборе типа EAP в качестве PEAP.|
|authenticationPeriodInSeconds|Int32|Укажите количество секунд, которые клиент должен ждать после попытки проверки подлинности перед сбоем. Допустимый диапазон 1-3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Укажите количество секунд между неудачной проверкой подлинности и следующей попыткой проверки подлинности. Допустимый диапазон 1-3600.|
|eapolStartPeriodInSeconds|Int32|Укажите количество секунд, которые необходимо подождать перед отправкой начните сообщение EAPOL (Extensible Authentication Protocol over LAN). Допустимый диапазон 1-3600.|
|maximumEAPOLStartMessages|Int32|Задано максимальное число протоколов проверки подлинности EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure. Допустимый диапазон 1-100.|
|maximumAuthenticationFailures|Int32|Укажите максимально допустимые сбои проверки подлинности для набора учетных данных. Допустимый диапазон 1-100.|
|cacheCredentials|Логический|Укажите, следует ли кэшизировать учетные данные пользователей на устройстве, чтобы пользователям не нужно было постоянно вводить их при каждом подключении.|
|authenticationType|[wifiAuthenticationType](../resources/intune-deviceconfig-wifiauthenticationtype.md)|Укажите, следует ли проверить подлинность пользователя, устройства или использовать гостевую проверку подлинности (нет). Если вы используете проверку подлинности сертификатов, убедитесь, что тип сертификата соответствует типу проверки подлинности. Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`.|

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
|rootCertificatesForServerValidation|[коллекция windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневой сертификат для проверки сервера. Эта коллекция может содержать не более 500 элементов.|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Укажите сертификат удостоверения для проверки подлинности клиента.|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневой сертификат для проверки клиента.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 1024,
  "authenticationRetryDelayPeriodInSeconds": 1024,
  "eapolStartPeriodInSeconds": 1024,
  "maximumEAPOLStartMessages": 1024,
  "maximumAuthenticationFailures": 1024,
  "cacheCredentials": true,
  "authenticationType": "String"
}
```



