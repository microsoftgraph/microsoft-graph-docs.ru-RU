---
title: Тип ресурса Девицеманажементскриптдевицестате
description: Содержит свойства для состояния запуска на устройстве скрипта управления устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbb088dbe6fc9e9cd324124269e4cfb8a4c7c66b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784911"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Тип ресурса Девицеманажементскриптдевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска на устройстве скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементскриптдевицестатес](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|Коллекция [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список свойств и связей объектов [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Получение Девицеманажементскриптдевицестате](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Чтение свойств и связей объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Создание Девицеманажементскриптдевицестате](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Создание нового объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|
|[Удаление Девицеманажементскриптдевицестате](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Нет|Удаляет объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[Обновление Девицеманажементскриптдевицестате](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md);|Обновление свойств объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния устройства сценария управления устройствами. Это свойство доступно только для чтения.|
|рунстате|[рунстате](../resources/intune-shared-runstate.md)|Состояние последнего запуска скрипта управления устройствами. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|ресултмессаже|String|Сведения о выходных данных выполнения.|
|ластстатеупдатедатетиме|DateTimeOffset|Последнее время выполнения скрипта управления устройствами.|
|errorCode|Int32|Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.|
|errorDescription|String|Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемые устройства, которые выполняют скрипт управления устройствами.|

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



