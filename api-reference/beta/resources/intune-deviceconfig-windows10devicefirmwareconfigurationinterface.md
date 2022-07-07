---
title: Тип ресурса windows10DeviceFirmwareConfigurationInterface
description: 'Свойства графа для интерфейса конфигурации встроенного ПО устройства '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db2c0e1b9a9815fd5882bd51364cbc2f285d37a7
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668400"
---
# <a name="windows10devicefirmwareconfigurationinterface-resource-type"></a>Тип ресурса windows10DeviceFirmwareConfigurationInterface

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства графа для интерфейса конфигурации встроенного ПО устройства 


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10DeviceFirmwareConfigurationInterfaces](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-list.md)|[Коллекция windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Список свойств и связей объектов [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Получение объекта windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-get.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Чтение свойств и связей объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Создание объекта windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-create.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Создайте объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Удаление объекта windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-delete.md)|Нет|Удаляет объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).|
|[Обновление windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-update.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Обновление свойств объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|Определяет уровень разрешений, предоставленный пользователям для изменения параметров UEFI. Возможные значения: `notConfiguredOnly`, `none`.|
|virtualizationOfCpuAndIO|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, включена ли виртуализация ЦП и ввода-вывода. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Камеры|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, включены ли встроенные камеры. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|microphonesAndSpeakers|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, включены ли встроенные микрофоны или динамики. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Радио|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, включены ли встроенные радиочастотные устройства, например WIFI, NFC, Bluetooth. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|bootFromExternalMedia|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешена ли пользователю загрузка с внешнего носителя. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|bootFromBuiltInNetworkAdapters|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешена ли пользователю загрузка из встроенных сетевых адаптеров. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|windowsPlatformBinaryTable|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить двоичную таблицу платформы Windows. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|simultaneousMultiThreading|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить одновременную многопоточность. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|frontCamera|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить front Camera. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|rearCamera|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить задняя камера. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|инфракрасная камеры|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить инфракрасную камеру. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Микрофон|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить микрофон. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Bluetooth|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включать Bluetooth. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wirelessWideAreaNetwork|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить беспроводную сеть с широкими областями. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|nearFieldCommunication|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить связь с полями, близкого к полю. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Wifi|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить Wi-Fi. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|usbTypeAPort|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить порт USB типа A. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Sdcard|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить порт SD Card. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wakeOnLAN|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить пробуждение по локальной сети. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wakeOnPower|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, разрешено ли пользователю включить wake On Power. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

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
  "bootFromBuiltInNetworkAdapters": "String",
  "windowsPlatformBinaryTable": "String",
  "simultaneousMultiThreading": "String",
  "frontCamera": "String",
  "rearCamera": "String",
  "infraredCamera": "String",
  "microphone": "String",
  "bluetooth": "String",
  "wirelessWideAreaNetwork": "String",
  "nearFieldCommunication": "String",
  "wiFi": "String",
  "usbTypeAPort": "String",
  "sdCard": "String",
  "wakeOnLAN": "String",
  "wakeOnPower": "String"
}
```




