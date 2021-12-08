---
title: тип ресурса hardwareConfigurationDeviceState
description: Содержит свойства для состояния запуска устройства конфигурации оборудования
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4700f48823a54bba155841b492e5ff139f05e235
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345622"
---
# <a name="hardwareconfigurationdevicestate-resource-type"></a>тип ресурса hardwareConfigurationDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска устройства конфигурации оборудования

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список hardwareConfigurationDeviceStates](../api/intune-deviceconfig-hardwareconfigurationdevicestate-list.md)|[коллекция hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Список свойств и связей объектов [hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Get hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-get.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Чтение свойств и связей объекта [hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Создание hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-create.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Создание нового [объекта hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Удаление hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-delete.md)|Нет|Удаляет [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md).|
|[Обновление оборудованияConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-update.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Обновление свойств объекта [hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша состояния состояния устройства конфигурации оборудования. Это свойство доступно только для чтения.|
|deviceName|String|Имя устройства|
|osVersion|String|Версия операционной системы устройства.|
|upn|String|Имя участника-пользователя (UPN).|
|internalVersion|Int32|Внутренняя версия Policy|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения конфигурации оборудования|
|configurationState|[runState](../resources/intune-shared-runstate.md)|Состояние конфигурации из последнего выполнения конфигурации оборудования. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|String|Выход выполнения конфигурации оборудования|
|configurationError|Строка|Ошибка при выполнении конфигурации оборудования|

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




