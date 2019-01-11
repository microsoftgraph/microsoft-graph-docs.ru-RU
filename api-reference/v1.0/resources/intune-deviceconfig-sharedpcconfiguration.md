---
title: Тип ресурса sharedPCConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом sharedPCConfiguration.
localization_priority: Normal
ms.openlocfilehash: a95c10a57751143f3ed4da19db6e351693fe0410
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862085"
---
# <a name="sharedpcconfiguration-resource-type"></a>Тип ресурса sharedPCConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом sharedPCConfiguration.

Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|Коллекция объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Получение объектов sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Чтение свойств и связей объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Создание объекта sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Создание объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Удаление объекта sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|Нет|Удаление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Обновление объекта sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Обновление свойств объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|описание|Строка|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|Задает способ управления учетными записями на общем компьютере. Применяется, только если для параметра disableAccountManager задано значение false.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|Указывает тип учетных записей, которые можно использовать на общем компьютере. Возможные значения: `guest`, `domain`.|
|allowLocalStorage|Boolean|Указывает, можно ли разместить локальное хранилище на общем компьютере.|
|disableAccountManager|Boolean|Отключает диспетчер учетных записей в режиме совместного использования компьютера.|
|disableEduPolicies|Boolean|Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования. Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.|
|disablePowerPolicies|Boolean|Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.|
|disableSignInOnResume|Boolean|Отключает обязательный вход в систему при выходе устройства из спящего режима.|
|enabled|Boolean|Включает режим общего компьютера и применяет политики совместного использования ПК.|
|idleTimeBeforeSleepInSeconds|Int32|Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим. Если задать значение 0, переход в спящий режим отключается.|
|kioskAppDisplayName|String|Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId. Применяется, только если задано свойство KioskAppUserModelId.|
|kioskAppUserModelId|String|Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.|
|maintenanceStartTime|TimeOfDay|Указывает ежедневное время начала обслуживания.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```



