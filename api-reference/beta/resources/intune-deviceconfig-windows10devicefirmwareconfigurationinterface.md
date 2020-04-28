---
title: Тип ресурса windows10DeviceFirmwareConfigurationInterface
description: 'Свойства Graph для интерфейса настройки встроенного по устройства '
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e53c408d31c53f0c0f4ebd76c0b4558160f0e1f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466929"
---
# <a name="windows10devicefirmwareconfigurationinterface-resource-type"></a>Тип ресурса windows10DeviceFirmwareConfigurationInterface

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства Graph для интерфейса настройки встроенного по устройства 


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10DeviceFirmwareConfigurationInterfaces](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-list.md)|Коллекция [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Список свойств и связей объектов [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Получение windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-get.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Чтение свойств и связей объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Создание windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-create.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Создание нового объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Удаление windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-delete.md)|Нет|Удаляет объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).|
|[Обновление windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-update.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Обновление свойств объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|Определяет уровень разрешений, который предоставляется пользователям для изменения параметров UEFI. Возможные значения: `notConfiguredOnly`, `none`.|
|виртуализатионофкпуандио|[Включение](../resources/intune-shared-enablement.md)|Определяет, включена ли виртуализация ЦП и ввода-вывода. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|камер|[Включение](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные камеры. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|микрофонесандспеакерс|[Включение](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные микрофоны или динамики. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Радио|[Включение](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные радиостанции, например Wi-Fi, NFC, Bluetooth. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|бутфромекстерналмедиа|[Включение](../resources/intune-shared-enablement.md)|Определяет, может ли пользователь загружаться с внешнего носителя. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|бутфромбуилтиннетворкадаптерс|[Включение](../resources/intune-shared-enablement.md)|Определяет, может ли пользователь загружаться со встроенных сетевых адаптеров. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10DeviceFirmwareConfigurationInterface"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "String",
  "virtualizationOfCpuAndIO": "String",
  "cameras": "String",
  "microphonesAndSpeakers": "String",
  "radios": "String",
  "bootFromExternalMedia": "String",
  "bootFromBuiltInNetworkAdapters": "String"
}
```



