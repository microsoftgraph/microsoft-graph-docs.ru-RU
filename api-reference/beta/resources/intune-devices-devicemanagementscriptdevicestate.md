---
title: тип ресурса deviceManagementScriptDeviceState
description: Содержит свойства для состояния запуска устройства скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90b9eaff6f291205acc559101e8ff4f64a33c8c8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611932"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>тип ресурса deviceManagementScriptDeviceState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска устройства скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список свойств и связей [объектов deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Get deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Чтение свойств и связей [объекта deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Создание deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Создайте новый [объект deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Удаление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Нет|Удаляет [устройствоManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[Обновление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Обновление свойств объекта [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния скрипта устройства управления устройствами. Это свойство доступно только для чтения.|
|runState|[runState](../resources/intune-devices-runstate.md)|Состояние последнего запуска сценария управления устройствами. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|String|Сведения о выходе выполнения.|
|lastStateUpdateDateTime|DateTimeOffset|Последний раз, когда выполняется скрипт управления устройствами.|
|errorCode|Int32|Код ошибки, соответствующий ошибочному исполнению сценария управления устройствами.|
|errorDescription|String|Описание ошибки, соответствующее ошибочному исполнению сценария управления устройствами.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемые устройства, которые выполняют сценарий управления устройствами.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```




