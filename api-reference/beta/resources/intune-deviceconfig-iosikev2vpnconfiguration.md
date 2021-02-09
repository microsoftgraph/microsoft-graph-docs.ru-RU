---
title: Тип ресурса iosikEv2VpnConfiguration
description: Укажет конфигурации в этом профиле, чтобы устройство с iOS подключилось к нужной конечной точке VPN IKEv2.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a99a4a6b0ab46a00ed44e0ca178c5e97cda050a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161798"
---
# <a name="iosikev2vpnconfiguration-resource-type"></a>Тип ресурса iosikEv2VpnConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Укажет конфигурации в этом профиле, чтобы устройство с iOS подключилось к нужной конечной точке VPN IKEv2.


Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosikEv2VpnConfigurations](../api/intune-deviceconfig-iosikev2vpnconfiguration-list.md)|[Коллекция iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Список свойств и связей объектов [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Get iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-get.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Чтение свойств и связей объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Создание iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-create.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Создание объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Удаление iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-delete.md)|Нет|Удаляет [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|
|[Обновление iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-update.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Обновление свойств объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли конфигурация устройства назначение тегов области. Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|connectionName|String|Имя подключения, отображаемая для пользователя. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Тип подключения. Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md) Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .|
|loginGroupOrDomain|String|Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|Роль, если для типа подключения установлено значение Pulse Secure. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|realm|String|Область, когда для типа подключения установлено "Pulse Secure". Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN-сервер в сети. Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|идентификатор|String|Идентификатор, предоставляемый поставщиком VPN, если для типа подключения установлено настраиваемая VPN-подключение. Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customData|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении. Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение. Эта коллекция может содержать не более 25 элементов. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пользовательские данные, если для типа подключения установлено настраиваемая VPN-сеть. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении. Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение". Эта коллекция может содержать не более 25 элементов. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|Boolean|Отправлять весь сетевой трафик через VPN. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Метод проверки подлинности для этого VPN-подключения. Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md) Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.|
|enablePerApp|Boolean|Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве пользователя с iOS. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|Коллекция String|Домены Safari, если этот параметр VPN для каждого приложения включен. Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)|Правила по запросу. Эта коллекция может содержать не более 500 элементов. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|Тип поставщика для VPN для каждого приложения. Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md) Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.|
|associatedDomains|Коллекция String|Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|excludedDomains|Коллекция String|Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disableOnDemandUserOverride|Boolean|Переключение, чтобы запретить пользователю отключать автоматическую VPN-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Прокси-сервер. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|Boolean|Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети. Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|userDomain|String|Только Zscaler. Введите статический домен для предварительного заполнения поля входа в приложение Zscaler. Если оставить его пустым, будет использоваться домен Azure Active Directory пользователя. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|strictEnforcement|Boolean|Только Zscaler. Блокирует сетевой трафик, пока пользователь не войди в приложение Zscaler. "True" означает, что трафик заблокирован. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|cloudName|String|Только Zscaler. Облако Zscaler, которому назначен пользователь. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|excludeList|Коллекция String|Только Zscaler. Список сетевых адресов, которые не отправляются через облако Zscaler. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|targetedMobileApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Целевые мобильные приложения. Эта коллекция может содержать не более 500 элементов. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|microsoftTunnelSiteId|String|Microsoft Tunnel site ID. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|childSecurityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Параметры связи между безопасностью и безопасностью|
|clientAuthenticationType|[vpnClientAuthenticationType](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|Тип проверки подлинности клиента, который будет использовать VPN-клиент. Возможные значения: `userAuthentication`, `deviceAuthentication`.|
|deadPeerDetectionRate|[vpnDeadPeerDetectionRate](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|Определите, как часто проверяется активность одноранговых подключений. . Возможные значения: `medium`, `none`, `low`, `high`.|
|disableMobilityAndMultihoming|Boolean|Отключение MOBIKE|
|disableRedirect|Boolean|Отключить перенаправление|
|enableCertificateRevocationCheck|Boolean|Включает проверку отзыва с наилучшими усилиями; Время отклика сервера не приведет к сбойу|
|enableEAP|Boolean|Включает только проверку подлинности EAP|
|enablePerfectForwardSecrecy|Boolean|Включить PFS.|
|enableUseInternalSubnetAttributes|Boolean|Включить использование атрибутов внутренней подсети.|
|localIdentifier|[vpnLocalIdentifier](../resources/intune-deviceconfig-vpnlocalidentifier.md)|Способ идентификации клиента, который пытается подключиться через VPN. . Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.|
|remoteIdentifier|String|Адрес сервера IKEv2. Должно быть FQDN, UserFQDN, сетевой адрес или ASN1DN|
|securityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Параметры ассоциации безопасности|
|serverCertificateCommonName|String|Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера|
|serverCertificateIssuerCommonName|String|Общее имя выпуска сертификата сервера IKEv2, используемого при проверке подлинности|
|serverCertificateType|[vpnServerCertificateType](../resources/intune-deviceconfig-vpnservercertificatetype.md)|Тип сертификата, который VPN-сервер будет представлять VPN-клиенту для проверки подлинности. Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.|
|sharedSecret|String|Используется при выборе проверки подлинности с общим секретом|
|tlsMaximumVersion|String|Максимальная версия TLS, используемая для проверки подлинности EAP-TLS|
|tlsMinimumVersion|String|Минимальная версия TLS, используемая для проверки подлинности EAP-TLS|
|allowDefaultSecurityAssociationParameters|Boolean|Разрешает использование параметров связи безопасности, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.|
|allowDefaultChildSecurityAssociationParameters|Boolean|Разрешает использование параметров связи между безопасностью, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.|
|alwaysOnConfiguration|[appleVpnAlwaysOnConfiguration](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|Конфигурация AlwaysOn|
|enableAlwaysOnConfiguration|Boolean|Определяет, включена ли always on VPN|
|mtuSizeInBytes|Int32|Максимальная единица передачи. Допустимые значения: от 1280 до 1400|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если методом проверки подлинности является сертификат. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, используемых для проверки подлинности. Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|

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




