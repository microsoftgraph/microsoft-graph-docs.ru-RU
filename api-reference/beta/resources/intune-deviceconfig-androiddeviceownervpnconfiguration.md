---
title: Тип ресурса androidDeviceOwnerVpnConfiguration
description: Указав конфигурации в этом профиле, можно указать полностью управляемому устройству Android подключиться к нужной конечной точке VPN. Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать VPN-подключение простым для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cb4fd59621583d69a1a8e0dc762625620fb76ed
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669807"
---
# <a name="androiddeviceownervpnconfiguration-resource-type"></a>Тип ресурса androidDeviceOwnerVpnConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указав конфигурации в этом профиле, можно указать полностью управляемому устройству Android подключиться к нужной конечной точке VPN. Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать VPN-подключение простым для конечного пользователя.


Наследует от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов androidDeviceOwnerVpnConfiguration](../api/intune-deviceconfig-androiddeviceownervpnconfiguration-list.md)|[Коллекция androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)|Список свойств и связей объектов [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .|
|[Получение объекта androidDeviceOwnerVpnConfiguration](../api/intune-deviceconfig-androiddeviceownervpnconfiguration-get.md)|[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)|Чтение свойств и связей объекта [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .|
|[Создание объекта androidDeviceOwnerVpnConfiguration](../api/intune-deviceconfig-androiddeviceownervpnconfiguration-create.md)|[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)|Создайте объект [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .|
|[Удаление объекта androidDeviceOwnerVpnConfiguration](../api/intune-deviceconfig-androiddeviceownervpnconfiguration-delete.md)|Нет|Удаляет [объект androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).|
|[Обновление объекта androidDeviceOwnerVpnConfiguration](../api/intune-deviceconfig-androiddeviceownervpnconfiguration-update.md)|[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)|Обновление свойств объекта [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Метод проверки подлинности. Наследуется [от vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md). Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.|
|connectionName|String|Имя подключения, отображаемое пользователю. Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)|
|role|String|Роль, если для типа подключения задано значение Pulse Secure. Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)|
|Realm|String|Область, если для типа подключения задано значение Pulse Secure. Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)|
|Серверов|[Коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Список VPN-серверов в сети. Убедитесь, что конечные пользователи имеют доступ к этим сетевым расположениям. Эта коллекция может содержать не более 500 элементов. Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)|
|connectionType|[androidVpnConnectionType](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|Тип подключения. Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Прокси-сервер.|
|targetedPackageIds|Коллекция строк|Идентификаторы пакетов целевых приложений.|
|targetedMobileApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Целевые мобильные приложения. Эта коллекция может содержать не более 500 элементов.|
|Alwayson|Логическое|Следует ли включить постоянное VPN-подключение.|
|alwaysOnLockdown|Логическое|Если включено постоянное VPN-подключение, следует ли блокировать сетевой трафик при отключении этого VPN.|
|microsoftTunnelSiteId|String|Идентификатор сайта Microsoft Tunnel.|
|Customdata|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Пользовательские данные для определения пар "ключ-значение", относящиеся к поставщику VPN. Эта коллекция может содержать не более 25 элементов.|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|Пользовательские данные для определения пар "ключ-значение", относящиеся к поставщику VPN. Эта коллекция может содержать не более 25 элементов.|

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
|identityCertificate|[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если методом проверки подлинности является сертификат.|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, используемых для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
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
  "authenticationMethod": "String",
  "connectionName": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "connectionType": "String",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "targetedPackageIds": [
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
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "String",
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
  ]
}
```




