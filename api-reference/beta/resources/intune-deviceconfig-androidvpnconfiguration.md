---
title: Тип ресурса androidVpnConfiguration
description: Укажет конфигурации в этом профиле, чтобы устройство Android подключилось к нужной конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение удобным для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e2396890f1f0a25ea59e72342b2f1f79efede62
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161560"
---
# <a name="androidvpnconfiguration-resource-type"></a>Тип ресурса androidVpnConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставив конфигурации в этом профиле, вы можете предоставить устройству Android указание подключиться к нужной конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение удобным для конечного пользователя.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidVpnConfigurations](../api/intune-deviceconfig-androidvpnconfiguration-list.md)|[Коллекция androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)|Список свойств и связей объектов [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)|
|[Get androidVpnConfiguration](../api/intune-deviceconfig-androidvpnconfiguration-get.md)|[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)|Чтение свойств и связей объекта [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)|
|[Создание androidVpnConfiguration](../api/intune-deviceconfig-androidvpnconfiguration-create.md)|[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)|Создание объекта [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)|
|[Удаление androidVpnConfiguration](../api/intune-deviceconfig-androidvpnconfiguration-delete.md)|Нет|Удаляет [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)|
|[Обновление androidVpnConfiguration](../api/intune-deviceconfig-androidvpnconfiguration-update.md)|[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)|Обновление свойств объекта [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|connectionName|String|Имя подключения, отображаемая для пользователя.|
|connectionType|[androidVpnConnectionType](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|Тип подключения. Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.|
|role|String|Роль, если для типа подключения установлено значение Pulse Secure.|
|realm|String|Область, когда для типа подключения установлено безопасное пульса.|
|серверы|[Коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Список VPN-серверов в сети. Убедитесь, что конечные пользователи имеют доступ к этим сетевым расположениям. Эта коллекция может содержать не более 500 элементов.|
|fingerprint|String|Отпечаток пальца — это строка, которая будет использоваться для проверки того, что VPN-сервер может быть доверенным, что применимо только в том случае, если типом подключения является VPN Check Point Vpn.|
|customData|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Пользовательские данные, если для типа подключения установлено citrix. Эта коллекция может содержать не более 25 элементов.|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пользовательские данные, если для типа подключения установлено citrix. Эта коллекция может содержать не более 25 элементов.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.|

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
|identityCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если методом проверки подлинности является сертификат.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
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
  "fingerprint": "String",
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
  "authenticationMethod": "String"
}
```




