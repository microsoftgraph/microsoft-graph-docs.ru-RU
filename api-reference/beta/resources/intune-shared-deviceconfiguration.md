---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b595f8fdcc680ff93693f0fcee7f618386aa0740
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201236"
---
# <a name="deviceconfiguration-resource-type"></a>Тип ресурса deviceConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация устройства

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceConfiguration](../api/intune-shared-deviceconfiguration-list.md)|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|[Получение объекта deviceConfiguration](../api/intune-shared-deviceconfiguration-get.md)|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|**Настройка устройства**|
|[Действие assign](../api/intune-shared-deviceconfiguration-assign.md)|Коллекция deviceConfigurationAssignment|Пока не задокументировано.|
|[Действие windowsPrivacyAccessControls](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|Нет|Н/Д|
|[Действие assignedAccessMultiModeProfiles](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|Нет|Н/Д|
|[Действие getTargetedUsersAndDevices](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|Коллекция Девицеконфигуратионтаржетедусеранддевице|Пока не задокументировано.|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|
|суппортсскопетагс|Boolean.|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения.|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики.|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики.|
|девицеманажементаппликабилитируледевицемоде|[девицеманажементаппликабилитируледевицемоде](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|description|String|Указанное администратором описание конфигурации устройства.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|**Настройка устройства**|
|groupAssignments|Коллекция deviceConfigurationGroupAssignment|Список назначений групп для профиля конфигурации устройства.|
|assignments|Коллекция объектов deviceConfigurationAssignment|Список назначений для профиля конфигурации устройства.|
|deviceStatuses|Коллекция deviceConfigurationDeviceStatus|Состояние установки конфигурации для каждого устройства.|
|userStatuses|Коллекция deviceConfigurationUserStatus|Состояние установки конфигурации устройств пользователем.|
|deviceStatusOverview|deviceConfigurationDeviceOverview|Обзор состояния конфигураций устройств|
|userStatusOverview|deviceConfigurationUserOverview|Обзор состояния конфигураций устройств по пользователям|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка по состоянию параметров конфигурации устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
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
  "version": 1024
}
```



