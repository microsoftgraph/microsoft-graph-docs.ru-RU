---
title: тип ресурса iosikEv2VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете поручить устройству iOS подключиться к нужной конечной точке VPN IKEv2.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68edc2108b8705f5cd6cc4021e8c28ed8342197e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111154"
---
# <a name="iosikev2vpnconfiguration-resource-type"></a>тип ресурса iosikEv2VpnConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете поручить устройству iOS подключиться к нужной конечной точке VPN IKEv2.


Наследуется [от iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosikEv2VpnConfigurations](../api/intune-deviceconfig-iosikev2vpnconfiguration-list.md)|[коллекция iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Список свойств и связей объектов [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Get iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-get.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Чтение свойств и связей объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Создание iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-create.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Создайте новый [объект iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Удаление iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-delete.md)|Нет|Удаляет [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).|
|[Обновление iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-update.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Обновление свойств объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|

## <a name="properties"></a>Свойства
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
|connectionName|String|Имя подключения, отображаемая пользователю. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Тип подключения. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Возможные значения: `ciscoAnyConnect` `pulseSecure` , , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` , , `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .|
|loginGroupOrDomain|String|Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|Роль при наборе типа подключения к Pulse Secure. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|realm|String|Realm, когда тип подключения за установлен в Pulse Secure. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN Server в сети. Убедитесь, что конечные пользователи могут получить доступ к этому расположению сети. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|идентификатор|String|Идентификатор, предоставляемый поставщиком VPN при наборе типа подключения к настраиваемой VPN. Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin, унаследованный от [appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customData|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Настраиваемые данные при наборе типа подключения к настраиваемой VPN. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении. Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений. Эта коллекция может содержать не более 25 элементов. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|Настраиваемые данные при наборе типа подключения к настраиваемой VPN. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении. Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений. Эта коллекция может содержать не более 25 элементов. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|Логическое|Отправка всего сетевого трафика через VPN. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Метод проверки подлинности для этого VPN-подключения. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.|
|enablePerApp|Логическое|Настройка этого параметра создает Per-App, которая впоследствии может быть связана с приложениями, которые могут запускать этот VPN-коннекцитон на устройстве iOS конечного пользователя. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|Коллекция объектов string|Домены Safari при включении этого параметра VPN для приложения. Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)|Правила по запросу. Эта коллекция может содержать не более 500 элементов. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|Тип поставщика для VPN-приложения. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.|
|associatedDomains|Коллекция объектов string|Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|excludedDomains|Коллекция объектов string|Домены, которые доступны через общедоступный интернет, а не через VPN, даже если VPN для каждого приложения активируется, наследуется [из appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disableOnDemandUserOverride|Логический|Чтобы предотвратить отключение автоматического VPN в приложении Параметры, унаследованной от [appleVpnConfiguration,](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdle|Логический|Отключение после простоя подключения по требованию, унаследованной от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdleTimerInSeconds|Int32|Время в секундах, необходимое для ожидания перед отключением подключения по запросу. Допустимые значения от 0 до 65535, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Прокси-сервер. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|Логическое|Opt-In совместное использование Id устройства сторонним vpn-клиентам для использования во время проверки контроля доступа к сети. Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|userDomain|String|Zscaler только. Введите статический домен для предварительного заполнения поля входа в приложение Zscaler. Если этот домен останется пустым, вместо него Azure Active Directory домен пользователя. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|strictEnforcement|Логическое|Zscaler только. Блокирует сетевой трафик до тех пор, пока пользователь не впишется в приложение Zscaler. "True" означает, что трафик заблокирован. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|cloudName|String|Zscaler только. Облако Zscaler, которому назначен пользователь. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|excludeList|Коллекция объектов string|Zscaler только. Список сетевых адресов, которые не отправляются через облако Zscaler. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|targetedMobileApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Целевые мобильные приложения. Эта коллекция может содержать не более 500 элементов. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|microsoftTunnelSiteId|String|Microsoft Tunnel сайта. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|childSecurityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Параметры ассоциации безопасности детей|
|clientAuthenticationType|[vpnClientAuthenticationType](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|Тип проверки подлинности клиента, который будет использовать VPN-клиент. Возможные значения: `userAuthentication`, `deviceAuthentication`.|
|deadPeerDetectionRate|[vpnDeadPeerDetectionRate](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|Определите, как часто проверять, активна ли одноранговая связь. . Возможные значения: `medium`, `none`, `low`, `high`.|
|disableMobilityAndMultihoming|Логический|Отключение MOBIKE|
|отключениеRedirect|Логический|Отключение перенаправления|
|enableCertificateRevocationCheck|Логическое|Включает проверку отзыва с наилучшими усилиями; Время ото времени отклика сервера не приведет к сбой|
|enableEAP|Логическое|Включает только проверку подлинности EAP|
|enablePerfectForwardSecrecy|Логический|Включить совершенную секретность вперед (PFS).|
|enableUseInternalSubnetAttributes|Логический|Включить использование атрибутов внутренней подсети.|
|localIdentifier|[vpnLocalIdentifier](../resources/intune-deviceconfig-vpnlocalidentifier.md)|Метод идентификации клиента, который пытается подключиться с помощью VPN. . Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.|
|remoteIdentifier|String|Адрес сервера IKEv2. Должен быть FQDN, UserFQDN, сетевой адрес или ASN1DN|
|securityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Параметры ассоциации безопасности|
|serverCertificateCommonName|String|Общее имя сертификата сервера IKEv2, используемого в проверке подлинности сервера|
|serverCertificateIssuerCommonName|String|Общее имя эмитента сертификата IKEv2 Server, используемого в проверке подлинности|
|serverCertificateType|[vpnServerCertificateType](../resources/intune-deviceconfig-vpnservercertificatetype.md)|Тип сертификата, который VPN-сервер представит VPN-клиенту для проверки подлинности. Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.|
|sharedSecret|String|Используется при выборе общей секретной проверки подлинности|
|tlsMaximumVersion|String|Максимальная версия TLS, используемая для проверки подлинности EAP-TLS|
|tlsMinimumVersion|String|Минимальная версия TLS, используемая для проверки подлинности EAP-TLS|
|allowDefaultSecurityAssociationParameters|Логический|Позволяет использовать параметры ассоциации безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано.|
|allowDefaultChildSecurityAssociationParameters|Логический|Позволяет использовать параметры ассоциации детской безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано.|
|alwaysOnConfiguration|[appleVpnAlwaysOnConfiguration](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|Конфигурация AlwaysOn|
|enableAlwaysOnConfiguration|Логическое|Определяет, включен ли always на VPN|
|mtuSizeInBytes|Int32|Максимальный блок передачи. Допустимые значения от 1280 до 1400|

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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Сертификат удостоверений для проверки подлинности клиента, когда метод проверки подлинности является сертификатом. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, которые будут использоваться для проверки подлинности. Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosikEv2VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "providerType": "String",
  "associatedDomains": [
    "String"
  ],
  "excludedDomains": [
    "String"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 1024,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true,
  "userDomain": "String",
  "strictEnforcement": true,
  "cloudName": "String",
  "excludeList": [
    "String"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "microsoftTunnelSiteId": "String",
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "clientAuthenticationType": "String",
  "deadPeerDetectionRate": "String",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "String",
  "remoteIdentifier": "String",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "serverCertificateCommonName": "String",
  "serverCertificateIssuerCommonName": "String",
  "serverCertificateType": "String",
  "sharedSecret": "String",
  "tlsMaximumVersion": "String",
  "tlsMinimumVersion": "String",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "String",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "String",
    "airPrintExceptionAction": "String",
    "cellularExceptionAction": "String",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "String"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 1024,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 1024
}
```



