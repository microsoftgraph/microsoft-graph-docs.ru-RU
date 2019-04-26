---
title: Тип ресурса Андроидомакпконфигуратион
description: Если вы предоставляете конфигурацию в этом профиле, вы можете настроить устройства Android, поддерживающие OMA — CP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c0e5edcbaabe0a363088eb0a21c5b9e4e416baa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556202"
---
# <a name="androidomacpconfiguration-resource-type"></a>Тип ресурса Андроидомакпконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Если вы предоставляете конфигурацию в этом профиле, вы можете настроить устройства Android, поддерживающие OMA — CP.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидомакпконфигуратионс](../api/intune-deviceconfig-androidomacpconfiguration-list.md)|Коллекция [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Список свойств и связей объектов [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Получение Андроидомакпконфигуратион](../api/intune-deviceconfig-androidomacpconfiguration-get.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Чтение свойств и связей объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Создание Андроидомакпконфигуратион](../api/intune-deviceconfig-androidomacpconfiguration-create.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Создание нового объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Удаление Андроидомакпконфигуратион](../api/intune-deviceconfig-androidomacpconfiguration-delete.md)|Нет|Удаляет объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md).|
|[Обновление Андроидомакпконфигуратион](../api/intune-deviceconfig-androidomacpconfiguration-update.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Обновление свойств объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Конфигуратионксмл|Двоичный|XML-файл конфигурации, который будет применен к устройству. При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.|

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

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidOmaCpConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "configurationXml": "binary"
}
```





