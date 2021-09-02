---
title: тип ресурса windows81WifiImportConfiguration
description: Windows 8.1+ Wi-Fi импортной конфигурации. Настройка этого профиля может Windows 8.1 (и более поздние) устройства для подключения к нужной Wi-Fi конечной точке. Подключение устройство Windows 8.1 в нужную сеть Wi-Fi и извлекает XML с этого устройства для более позднего встраиваемого Wi-Fi профиля.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca037ceae79a79bf7e25a8d5d8315651e8dd9c75
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786343"
---
# <a name="windows81wifiimportconfiguration-resource-type"></a>тип ресурса windows81WifiImportConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows 8.1+ Wi-Fi импортной конфигурации. Настройка этого профиля может Windows 8.1 (и более поздние) устройства для подключения к нужной Wi-Fi конечной точке. Подключение устройство Windows 8.1 в нужную сеть Wi-Fi и извлекает XML с этого устройства для более позднего встраиваемого Wi-Fi профиля.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows81WifiImportConfigurations](../api/intune-deviceconfig-windows81wifiimportconfiguration-list.md)|[коллекция windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|Список свойств и связей объектов [Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|
|[Get windows81WifiImportConfiguration](../api/intune-deviceconfig-windows81wifiimportconfiguration-get.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|Чтение свойств и связей [объекта Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|
|[Создание windows81WifiImportConfiguration](../api/intune-deviceconfig-windows81wifiimportconfiguration-create.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|Создайте [новый объект Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|
|[Удаление windows81WifiImportConfiguration](../api/intune-deviceconfig-windows81wifiimportconfiguration-delete.md)|Нет|Удаляет [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).|
|[Обновление windows81WifiImportConfiguration](../api/intune-deviceconfig-windows81wifiimportconfiguration-update.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|Обновление свойств объекта [Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|payloadFileName|String|Имя файла полезной нагрузки (*.xml).|
|имя профиля|Строка|Имя профиля, отображаемая в пользовательском интерфейсе.|
|payload|Binary|Полезные данные (массив byte, кодируемый UTF8). Это XML-файл, сохраненный на устройстве, с помощью Wi-Fi конечной точки.|

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
  "@odata.type": "microsoft.graph.windows81WifiImportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "String",
  "profileName": "String",
  "payload": "binary"
}
```



