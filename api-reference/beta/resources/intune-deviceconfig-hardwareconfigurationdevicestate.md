---
title: тип ресурса hardwareConfigurationDeviceState
description: Содержит свойства для состояния запуска устройства конфигурации оборудования
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70a5fdd114afd1ad4de4e6317282146f481e0288
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368275"
---
# <a name="hardwareconfigurationdevicestate-resource-type"></a>тип ресурса hardwareConfigurationDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска устройства конфигурации оборудования

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список hardwareConfigurationDeviceStates](../api/intune-deviceconfig-hardwareconfigurationdevicestate-list.md)|[коллекция hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Список свойств и связей объектов [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Get hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-get.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Чтение свойств и связей объекта [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Создание hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-create.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Создание нового [объекта hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Удаление hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-delete.md)|Нет|Удаляет [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md).|
|[Обновление оборудованияConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-update.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Обновление свойств объекта [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша состояния состояния устройства конфигурации оборудования. Это свойство доступно только для чтения.|
|deviceName|String|Имя устройства|
|osVersion|String|Версия операционной системы устройства (например. 10.0.19042.1165, 10.0.19042.1288 и т.д.)|
|upn|String|Имя участника-пользователя (UPN).|
|internalVersion|Int32|Внутренняя версия Policy|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения конфигурации оборудования|
|configurationState|[runState](../resources/intune-deviceconfig-runstate.md)|Состояние конфигурации из последнего выполнения конфигурации оборудования. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|Строка|Выход выполнения конфигурации оборудования|
|configurationError|String|Ошибка при выполнении конфигурации оборудования|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "String (identifier)",
  "deviceName": "String",
  "osVersion": "String",
  "upn": "String",
  "internalVersion": 1024,
  "lastStateUpdateDateTime": "String (timestamp)",
  "configurationState": "String",
  "configurationOutput": "String",
  "configurationError": "String"
}
```




