---
title: Тип ресурса Макоссофтвареупдатеконфигуратион
description: Конфигурация обновления программного обеспечения MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f1712a59ef6659ce6ac5e16f6111998fcf3455e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731101"
---
# <a name="macossoftwareupdateconfiguration-resource-type"></a>Тип ресурса Макоссофтвареупдатеконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация обновления программного обеспечения MacOS


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макоссофтвареупдатеконфигуратионс](../api/intune-deviceconfig-macossoftwareupdateconfiguration-list.md)|Коллекция [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Список свойств и связей объектов [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .|
|[Получение Макоссофтвареупдатеконфигуратион](../api/intune-deviceconfig-macossoftwareupdateconfiguration-get.md)|[макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Чтение свойств и связей объекта [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .|
|[Создание Макоссофтвареупдатеконфигуратион](../api/intune-deviceconfig-macossoftwareupdateconfiguration-create.md)|[макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Создание нового объекта [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .|
|[Удаление Макоссофтвареупдатеконфигуратион](../api/intune-deviceconfig-macossoftwareupdateconfiguration-delete.md)|Нет|Удаляет объект [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md).|
|[Обновление Макоссофтвареупдатеконфигуратион](../api/intune-deviceconfig-macossoftwareupdateconfiguration-update.md)|[макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Обновление свойств объекта [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|критикалупдатебехавиор|[макоссофтвареупдатебехавиор](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Обновление поведения критических обновлений. Возможные значения: `notConfigured`, `default`.|
|конфигдатаупдатебехавиор|[макоссофтвареупдатебехавиор](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Обновление поведения обновлений файлов данных конфигурации. Возможные значения: `notConfigured`, `default`.|
|фирмвареупдатебехавиор|[макоссофтвареупдатебехавиор](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Обновление поведения обновлений микропрограммного обеспечения. Возможные значения: `notConfigured`, `default`.|
|аллосерупдатебехавиор|[макоссофтвареупдатебехавиор](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Обновление поведения для всех остальных обновлений. Возможные значения: `notConfigured`, `default`.|
|упдатесчедулетипе|[макоссофтвареупдатесчедулетипе](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|Обновление типа расписания. Возможные значения: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.|
|кустомупдатетимевиндовс|Коллекция [кустомупдатетимевиндов](../resources/intune-deviceconfig-customupdatetimewindow.md)|Настраиваемое время Windows, когда обновления будут разрешены или заблокированы. Эта коллекция может содержать не более 20 элементов.|
|упдатетимевиндовуткоффсетинминутес|Int32|Минуты, указывающие смещение UTC для каждого периода обновления|

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
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "String",
  "configDataUpdateBehavior": "String",
  "firmwareUpdateBehavior": "String",
  "allOtherUpdateBehavior": "String",
  "updateScheduleType": "String",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "String",
      "endDay": "String",
      "startTime": "String (time of day)",
      "endTime": "String (time of day)"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 1024
}
```





