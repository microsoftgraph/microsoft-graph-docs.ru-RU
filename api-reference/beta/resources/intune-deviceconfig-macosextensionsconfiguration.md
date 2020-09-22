---
title: Тип ресурса Макосекстенсионсконфигуратион
description: Профиль конфигурации расширений MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c75959a5fdd45f9e351ff227f6c834837079b2c5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024187"
---
# <a name="macosextensionsconfiguration-resource-type"></a>Тип ресурса Макосекстенсионсконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации расширений MacOS.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосекстенсионсконфигуратионс](../api/intune-deviceconfig-macosextensionsconfiguration-list.md)|Коллекция [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Список свойств и связей объектов [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .|
|[Получение Макосекстенсионсконфигуратион](../api/intune-deviceconfig-macosextensionsconfiguration-get.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Чтение свойств и связей объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .|
|[Создание Макосекстенсионсконфигуратион](../api/intune-deviceconfig-macosextensionsconfiguration-create.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Создание нового объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .|
|[Удаление Макосекстенсионсконфигуратион](../api/intune-deviceconfig-macosextensionsconfiguration-delete.md)|Нет|Удаляет объект [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md).|
|[Обновление Макосекстенсионсконфигуратион](../api/intune-deviceconfig-macosextensionsconfiguration-update.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Обновление свойств объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|кернелекстенсионоверридесалловед|Boolean|Если задано значение true, пользователи могут утверждать дополнительные расширения ядра, не разрешенные профилями конфигураций.|
|кернелекстенсионалловедтеамидентифиерс|Коллекция String|Все расширения ядра, подписанные с помощью идентификаторов команд в этом списке, могут быть загружены.|
|кернелекстенсионсалловед|Коллекция [макоскернелекстенсион](../resources/intune-deviceconfig-macoskernelextension.md)|Список расширений ядра, которые будут разрешены для загрузки. . Эта коллекция может содержать не более 500 элементов.|
|системекстенсионсблокковерриде|Boolean|Получает или задает значение, указывающее, следует ли разрешить пользователю утверждать дополнительные системные расширения, которые явно не разрешены профилями конфигурации.|
|системекстенсионсалловедтеамидентифиерс|Коллекция String|Получает или задает список разрешенных идентификаторов групп. Все системные расширения, подписанные с помощью любого из указанных идентификаторов, будут утверждены.|
|системекстенсионсалловед|Коллекция [макоссистемекстенсион](../resources/intune-deviceconfig-macossystemextension.md)|Получает или задает список разрешенных расширений системы macOS. Эта коллекция может содержать не более 500 элементов.|
|системекстенсионсалловедтипес|Коллекция [макоссистемекстенсионтипемаппинг](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)|Получает или задает список разрешенных типов расширений системы macOS. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Отношения
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
  "@odata.type": "microsoft.graph.macOSExtensionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "String"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "String",
      "bundleId": "String"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "String"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "String",
      "bundleId": "String"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "String",
      "allowedTypes": "String"
    }
  ]
}
```






