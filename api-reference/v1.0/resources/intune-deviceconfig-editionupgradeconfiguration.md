---
title: Тип ресурса editionUpgradeConfiguration
description: Конфигурация обновления выпуска Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd1b02843826cb1e492f7a7897666b508d54daab
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457626"
---
# <a name="editionupgradeconfiguration-resource-type"></a>Тип ресурса editionUpgradeConfiguration

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация обновления выпуска Windows 10.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление editionUpgradeConfigurations](../api/intune-deviceconfig-editionupgradeconfiguration-list.md)|Коллекция [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Список свойств и связей объектов [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|
|[Получение editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-get.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Считывание свойств и связей объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|
|[Создание editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-create.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|
|[Удаление editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-delete.md)|None|Удаление экземпляра [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|
|[Обновление editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-update.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|licenseType|[editionUpgradeLicenseType](../resources/intune-deviceconfig-editionupgradelicensetype.md)|Тип лицензии для обновления выпуска. Возможные значения: `productKey`, `licenseFile`.|
|targetEdition|[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)|Целевой выпуск для обновления. Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.|
|license|String|Содержимое файла лицензии для обновления выпуска.|
|productKey|String|Ключ продукта для обновления выпуска.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.editionUpgradeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "String",
  "productKey": "String"
}
```



