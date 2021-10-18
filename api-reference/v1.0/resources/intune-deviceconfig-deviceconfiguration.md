---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 35e2101ace3a3f16da17acd09772c6fcf291c764
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451192"
---
# <a name="deviceconfiguration-resource-type"></a>Тип ресурса deviceConfiguration

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация устройства

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceConfiguration](../api/intune-deviceconfig-deviceconfiguration-list.md)|Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|[Получение объекта deviceConfiguration](../api/intune-deviceconfig-deviceconfiguration-get.md)|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|[Действие assign](../api/intune-deviceconfig-deviceconfiguration-assign.md)|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Н/Д|
|[функция getOmaSettingPlainTextValue](../api/intune-deviceconfig-deviceconfiguration-getomasettingplaintextvalue.md)|String|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|description|String|Указанное администратором описание конфигурации устройства.|
|displayName|String|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства.|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства.|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем.|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигураций устройств|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигураций устройств по пользователям|
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
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



