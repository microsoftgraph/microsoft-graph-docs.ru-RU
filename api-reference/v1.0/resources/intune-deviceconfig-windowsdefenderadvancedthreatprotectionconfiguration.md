---
title: Тип ресурса windowsDefenderAdvancedThreatProtectionConfiguration
description: Конфигурация Advanced Threat Protection в Защитника Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e66a21b9de53a8b93c74b1034784ea00fb514942
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256345"
---
# <a name="windowsdefenderadvancedthreatprotectionconfiguration-resource-type"></a>Тип ресурса windowsDefenderAdvancedThreatProtectionConfiguration

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация Advanced Threat Protection в Защитника Windows.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration-list.md)|Коллекция [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md)|Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration-get.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md);|Чтение свойств и связей объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration-create.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md);|Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Удаление объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration-delete.md)|Нет|Удаляет объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration-update.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md)|Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|allowSampleSharing|Логический|Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows|
|enableExpeditedTelemetryReporting|Boolean|Повышение частоты отправки отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



