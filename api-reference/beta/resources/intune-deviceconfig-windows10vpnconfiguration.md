---
title: тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете поручить Windows 10 (настольный компьютер или мобильный) подключиться к нужной конечной точке VPN. Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать подключение VPN бесшовным для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 644708037a7ae35cdd9e7787a0d583ed23840367
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801517"
---
# <a name="windows10vpnconfiguration-resource-type"></a>тип ресурса windows10VpnConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете поручить Windows 10 (настольный компьютер или мобильный) подключиться к нужной конечной точке VPN. Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать подключение VPN бесшовным для конечного пользователя.


Наследуется [от windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|[коллекция windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Список свойств и связей [объектов Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|
|[Получить windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Чтение свойств и связей [объекта Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|
|[Создание windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Создайте [новый объект Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|
|[Удаление windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|Нет|Удаляет [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).|
|[Обновление windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Обновление свойств объекта [Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|

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
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|connectionName|Строка|Имя подключения, отображаемая пользователю. Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|серверы|[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Список VPN-серверов в сети. Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям. Эта коллекция может содержать не более 500 элементов. Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|В двоичном формате|Настраиваемые XML-команды, настраиваемые vpn-подключением. (массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|profileTarget|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|Тип целевого профиля. Возможные значения: `user`, `device`, `autoPilotDevice`.|
|connectionType|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|Тип подключения. Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.|
|enableSplitTunneling|Логический|Включить раздельный туннель.|
|enableAlwaysOn|Логический|Включить режим Always On.|
|enableDeviceTunnel|Логический|Включить туннель устройства.|
|enableDnsRegistration|Логический|Включить регистрацию IP-адресов с помощью внутреннего DNS.|
|dnsSuffixes|Коллекция String|Укажите суффиксы DNS, чтобы добавить их в список поиска DNS, чтобы правильно маршрутизировать короткие имена.|
|authenticationMethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|Метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.|
|rememberUserCredentials|Логический|Помните учетные данные пользователей.|
|enableConditionalAccess|Логический|Включить условный доступ.|
|enableSingleSignOnWithAlternateCertificate|Логический|Включить один вход (SSO) с помощью альтернативного сертификата.|
|singleSignOnEku|[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)|Использование расширенного ключа с одним входом (EKU).|
|singleSignOnIssuerHash|Строка|Hash одного входного эмитента.|
|eapXml|В двоичном формате|XML-протокол экстратензивной проверки подлинности (EAP). (массив байтов в кодировке UTF8).|
|proxyServer|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|Прокси-сервер.|
|associatedApps|[коллекция windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)|Связанные приложения. Эта коллекция может содержать не более 10 000 элементов.|
|onlyAssociatedAppsCanUseConnection|Логический|Только связанные приложения могут использовать подключение (VPN для каждого приложения).|
|windowsInformationProtectionDomain|String|Windows Домен Защиты информации (WIP) для связи с этим подключением.|
|trafficRules|[коллекция vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)|Правила дорожного движения. Эта коллекция может содержать не более 1000 элементов.|
|маршруты|[коллекция vpnRoute](../resources/intune-deviceconfig-vpnroute.md)|Маршруты (необязательные для сторонних поставщиков). Эта коллекция может содержать не более 1000 элементов.|
|dnsRules|[коллекция vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)|Правила DNS. Эта коллекция может содержать не более 1000 элементов.|
|trustedNetworkDomains|Коллекция String|Доверенные сетевые домены|
|cryptographySuite|[cryptographySuite](../resources/intune-deviceconfig-cryptographysuite.md)|Параметры безопасности пакета шифрования для VPN IKEv2 в Windows10 и выше |

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
|identityCertificate|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Сертификат удостоверений для проверки подлинности клиента, когда метод проверки подлинности является сертификатом.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "String",
    "integrityCheckMethod": "String",
    "dhGroup": "String",
    "cipherTransformConstants": "String",
    "authenticationTransformConstants": "String",
    "pfsGroup": "String"
  }
}
```



