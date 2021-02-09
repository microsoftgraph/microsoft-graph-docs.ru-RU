---
title: Тип ресурса deviceManagementScriptDeviceState
description: Содержит свойства состояния запуска устройства сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bcce9f566f9f187bf55b8b201ee9ae29f7b627e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158500"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Тип ресурса deviceManagementScriptDeviceState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния запуска устройства сценария управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[Коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список свойств и связей объектов [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Get deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Чтение свойств и связей объекта [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Создание deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Создание объекта [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Удаление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Нет|Удаляет [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|
|[Обновление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Обновление свойств объекта [deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния устройства сценария управления устройствами. Это свойство доступно только для чтения.|
|runState|[runState](../resources/intune-shared-runstate.md)|Состояние последнего запуска сценария управления устройствами. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|String|Сведения о выходных данных выполнения.|
|lastStateUpdateDateTime|DateTimeOffset|Последнее время выполнения сценария управления устройствами.|
|errorCode|Int32|Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.|
|errorDescription|String|Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-shared-manageddevice.md);|Управляемые устройства, которые выполняют сценарий управления устройствами.|

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




