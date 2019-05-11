---
title: Тип ресурса Иосдериведкредентиалаусентикатионконфигуратион
description: Профиль производных учетных данных iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1aa7bab23f6c90420e262bed0c5a3f8a72cbbb51
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957101"
---
# <a name="iosderivedcredentialauthenticationconfiguration-resource-type"></a>Тип ресурса Иосдериведкредентиалаусентикатионконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль производных учетных данных iOS.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосдериведкредентиалаусентикатионконфигуратионс](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-list.md)|Коллекция [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|Список свойств и связей объектов [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .|
|[Получение Иосдериведкредентиалаусентикатионконфигуратион](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-get.md)|[Иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|Чтение свойств и связей объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .|
|[Создание Иосдериведкредентиалаусентикатионконфигуратион](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-create.md)|[Иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|Создание нового объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .|
|[Удаление Иосдериведкредентиалаусентикатионконфигуратион](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-delete.md)|Нет|Удаляет объект [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).|
|[Обновление Иосдериведкредентиалаусентикатионконфигуратион](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-update.md)|[Иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|Обновление свойств объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Дериведкредентиалсеттингс|[Девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, которые необходимо использовать для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDerivedCredentialAuthenticationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```




