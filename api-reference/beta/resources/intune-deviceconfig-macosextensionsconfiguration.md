---
title: тип ресурса macOSExtensionsConfiguration
description: Профиль конфигурации расширений MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d9565b4d2301c7e6896ded1b0fff250de2c994a19abf051452ee0a01775e117
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239562"
---
# <a name="macosextensionsconfiguration-resource-type"></a>тип ресурса macOSExtensionsConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации расширений MacOS.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSExtensionsConfigurations](../api/intune-deviceconfig-macosextensionsconfiguration-list.md)|[коллекция macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Список свойств и связей объектов [macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Get macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-get.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Чтение свойств и связей объекта [macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Создание macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-create.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Создайте [новый объект macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Удаление macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-delete.md)|Нет|Удаляет [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).|
|[Обновление macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-update.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Обновление свойств объекта [macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|kernelExtensionOverridesAllowed|Логический|Если установлено, что это так, пользователи могут утверждать дополнительные расширения ядра, явно не разрешенные профилями конфигураций.|
|kernelExtensionAllowedTeamIdentifiers|Коллекция String|Все расширения ядра, действительно подписанные идентификаторами группы в этом списке, будут разрешены для загрузки.|
|kernelExtensionsAllowed|[коллекция macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)|Список расширений ядра, которые можно загрузить. . Эта коллекция может содержать не более 500 элементов.|
|systemExtensionsBlockOverride|Логический|Получает или задает, разрешить ли пользователю утверждать дополнительные расширения системы, явно не разрешенные профилями конфигурации.|
|systemExtensionsAllowedTeamIdentifiers|Коллекция String|Получает или задает список разрешенных идентификаторов группы. Любое расширение системы, подписанное с любым из указанных идентификаторов группы, будет утверждено.|
|systemExtensionsAllowed|[коллекция macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md)|Получает или задает список разрешенных расширений системы macOS. Эта коллекция может содержать не более 500 элементов.|
|systemExtensionsAllowedTypes|[коллекция macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)|Получает или задает список разрешенных типов расширения системы macOS. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
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




