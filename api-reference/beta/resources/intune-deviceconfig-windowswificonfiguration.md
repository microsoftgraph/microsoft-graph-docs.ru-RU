---
title: Тип ресурса Виндовсвификонфигуратион
description: Конфигурация устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d735d5dcec50323323550c82f3bdbcccbd93f4b7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774171"
---
# <a name="windowswificonfiguration-resource-type"></a>Тип ресурса Виндовсвификонфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация устройства


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсвификонфигуратионс](../api/intune-deviceconfig-windowswificonfiguration-list.md)|Коллекция [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|Список свойств и связей объектов [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Получение Виндовсвификонфигуратион](../api/intune-deviceconfig-windowswificonfiguration-get.md)|[Виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|Чтение свойств и связей объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Создание Виндовсвификонфигуратион](../api/intune-deviceconfig-windowswificonfiguration-create.md)|[Виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|Создание нового объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Удаление Виндовсвификонфигуратион](../api/intune-deviceconfig-windowswificonfiguration-delete.md)|Нет|Удаляет объект [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).|
|[Обновление Виндовсвификонфигуратион](../api/intune-deviceconfig-windowswificonfiguration-update.md)|[Виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|Обновление свойств объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|preSharedKey|String|Это предварительно общий ключ для частной сети Wi-Fi WPA.|
|Вифисекурититипе|[Вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Укажите тип безопасности Wi-Fi. Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|Метередконнектионлимит|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Указать тип лимита межлимитного подключения для подключения WiFi. Возможные значения: `unrestricted`, `fixed`, `variable`.|
|SSID|String|Укажите идентификатор SSID подключения WiFi.|
|Нетворкнаме|String|Укажите имя конфигурации сети.|
|Коннектаутоматикалли|Boolean|Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.|
|Коннекттопреферреднетворк|Boolean|Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.  Необходимо, чтобы Коннектаутоматикалли был true.|
|Коннектвхеннетворкнамеишидден|Boolean|Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.|
|Проксисеттинг|[Вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Укажите параметры прокси-сервера для конфигурации Wi-Fi. Возможные значения: `none`, `manual`, `automatic`.|
|Проксимануаладдресс|String|Укажите IP-адрес прокси-сервера.|
|Проксимануалпорт|Int32|Укажите порт прокси-сервера.|
|Проксяутоматикконфигуратионурл|String|Укажите URL-адрес скрипта настройки прокси-сервера.|
|Форцефипскомплианце|Boolean|Укажите, следует ли применять соответствие требованиям FIPS.|

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

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "forceFIPSCompliance": true
}
```





