---
title: Тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88d32aedb16516f7659ff6e8094172e4a59f6345
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572019"
---
# <a name="windows10vpnconfiguration-resource-type"></a>Тип ресурса windows10VpnConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.


НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|Коллекция [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Получение windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Создание windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Удаление windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|Нет|Удаляет объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).|
|[Обновление windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Коннектионнаме|String|Имя подключения, отображаемое для пользователя. НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|серверами|Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)|Список VPN-серверов в сети. Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям. Эта коллекция может содержать не более 500 элементов. НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Двоичный|Настраиваемые XML-команды, которые настраивают VPN-подключение. (Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|Профилетаржет|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|Тип целевого объекта профиля. Возможные значения: `user`, `device`, `autoPilotDevice`.|
|connectionType|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|Тип подключения. Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.|
|Енаблесплиттуннелинг|Boolean|Включение Расщепленного туннелирования.|
|Енаблеалвайсон|Boolean|Включение режима "всегда включено".|
|Енабледевицетуннел|Boolean|Включите туннель устройства.|
|Енабледнсрегистратион|Boolean|Включить регистрацию IP-адресов с использованием внутренней DNS.|
|Днссуффиксес|Коллекция String|Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.|
|Параметр authenticationmethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|Метод проверки поДлинности. Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.|
|Ремемберусеркредентиалс|Boolean|Запомнить учетные данные пользователя.|
|Енаблекондитионалакцесс|Boolean|Включение условного доступа.|
|Енаблесинглесигнонвисалтернатецертификате|Boolean|Включите единый вход (SSO) с альтернативным сертификатом.|
|Синглесигнонеку|[Екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)|Расширенное использование ключа (EKU) единого входа.|
|Синглесигнониссуерхаш|String|Хэш поставщика единого входа.|
|Еапксмл|Двоичный|XML-файл протокола расширенной проверки поДлинности (EAP). (массив байтов в кодировке UTF8).|
|проксисервер|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|Прокси-сервер.|
|АссоЦиатедаппс|Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)|Связанные приложения. Эта коллекция может содержать не более 10 000 элементов.|
|ОнляссоЦиатедаппсканусеконнектион|Boolean|Подключение можно использовать только для связанных приложений (VPN для каждого приложения).|
|Виндовсинформатионпротектиондомаин|String|Домен Windows Information Protection (WIP) для связи с этим подключением.|
|Траффикрулес|Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)|Правила трафика. Эта коллекция может содержать не более 1000 элементов.|
|сылает|Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)|Маршруты (необязательно для сторонних поставщиков). Эта коллекция может содержать не более 1000 элементов.|
|Днсрулес|Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)|Правила DNS. Эта коллекция может содержать не более 1000 элементов.|
|trustedNetworkDomains|Коллекция String|Доверенные сетевые домены|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Identitycertificate (|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.|

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
  ]
}
```





