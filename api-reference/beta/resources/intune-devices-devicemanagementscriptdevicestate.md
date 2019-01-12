---
title: Тип ресурса deviceManagementScriptDeviceState
description: Содержит свойства для устройства, состояние сценарий управления устройства выполнения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f50026e549e9927b33ebe8a27b6206daecf0ea5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968857"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Тип ресурса deviceManagementScriptDeviceState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для устройства, состояние сценарий управления устройства выполнения.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) коллекции|Свойства списка и связей объектов [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Получение deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Чтение свойства и связи объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Создание deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Создание нового объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Удаление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Нет|Удаляет [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[Обновление deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Обновление свойства объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности состояния устройства устройства управления скрипта.|
|runState|[runState](../resources/intune-shared-runstate.md)|Состояние последнего выполнения сценарий управления устройства. Возможные значения: `unknown`, `success`, `fail`.|
|resultMessage|String|Подробные сведения о результатов выполнения.|
|lastStateUpdateDateTime|DateTimeOffset|Время последнего выполняет сценарий управления устройства.|
|errorCode|Int32|Код ошибки, соответствующий ошибочный выполнение сценария управления устройства.|
|errorDescription|String|Описание ошибки, соответствующий ошибочный выполнение сценария управления устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice;|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемые устройства, которые выполняет сценарий управления устройства.|

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





