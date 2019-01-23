---
title: Тип ресурса androidForWorkVpnConfiguration
description: С указанием конфигураций в этом профиле можно указать Android устройства для подключения к требуемой конечной точки VPN. Путем указания типов безопасности и метод проверки подлинности ожидаемого конечной точкой виртуальной частной сети VPN-подключение можно сделать полностью для конечных пользователей.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06172d66a3d2eecebe6581ed5cded2acb0755a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396142"
---
# <a name="androidforworkvpnconfiguration-resource-type"></a>Тип ресурса androidForWorkVpnConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

С указанием конфигураций в этом профиле можно указать Android устройства для подключения к требуемой конечной точки VPN. Путем указания типов безопасности и метод проверки подлинности ожидаемого конечной точкой виртуальной частной сети VPN-подключение можно сделать полностью для конечных пользователей.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidForWorkVpnConfigurations](../api/intune-deviceconfig-androidforworkvpnconfiguration-list.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) коллекции|Свойства списка и связей объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .|
|[Получение androidForWorkVpnConfiguration](../api/intune-deviceconfig-androidforworkvpnconfiguration-get.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md);|Чтение свойства и связи объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .|
|[Создание androidForWorkVpnConfiguration](../api/intune-deviceconfig-androidforworkvpnconfiguration-create.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md);|Создание нового объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .|
|[Удаление androidForWorkVpnConfiguration](../api/intune-deviceconfig-androidforworkvpnconfiguration-delete.md)|Нет|Удаляет [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).|
|[Обновление androidForWorkVpnConfiguration](../api/intune-deviceconfig-androidforworkvpnconfiguration-update.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md);|Обновление свойства объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|connectionName|String|Имя подключения отображается для пользователя.|
|Тип подключения|[androidForWorkVpnConnectionType](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|Тип подключения. Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.|
|role|String|Роль, если тип подключения для обеспечения безопасности Pulse.|
|область|String|Область, если тип подключения для обеспечения безопасности Pulse.|
|серверы|[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции|Список VPN-серверов в сети. Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети. Эта коллекция может содержать не более 500 элементов.|
|отпечаток пальца|String|Отпечаток является строку, которая будет использоваться для проверки VPN-сервер может быть доверенным, который применяется только для проверки VPN капсула точка — это тип подключения.|
|customData|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Пользовательские данные Citrix задается тип подключения. Эта коллекция может содержать не более 25 элементов.|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пользовательские данные Citrix задается тип подключения. Эта коллекция может содержать не более 25 элементов.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиентов, если метод проверки подлинности сертификата.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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




