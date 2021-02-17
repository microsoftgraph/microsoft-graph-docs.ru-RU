---
title: Тип ресурса deviceComplianceScriptDeviceState
description: Содержит свойства состояния выполнения устройства для сценария соответствия устройств требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db40c6412f022ce9ba94619005ab2ebcf60e3dab
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272186"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a>Тип ресурса deviceComplianceScriptDeviceState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния выполнения устройства для сценария соответствия устройств требованиям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceComplianceScriptDeviceStates](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|[Коллекция deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список свойств и связей объектов [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Get deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Чтение свойств и связей объекта [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Создание deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Создание объекта [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Удаление deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|Нет|Удаляет [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Обновление deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Обновление свойств объекта [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния устройства для сценария соответствия требованиям. Это свойство доступно только для чтения.|
|detectionState|[runState](../resources/intune-shared-runstate.md)|Состояние обнаружения из последнего выполнения сценария соответствия устройств требованиям. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|Последняя временная запамяка выполнения сценария соответствия устройств требованиям|
|expectedStateUpdateDateTime|DateTimeOffset|Следующая временная заметив, когда ожидается выполнение сценария соответствия устройств требованиям|
|lastSyncDateTime|DateTimeOffset|Время последней синхронизации расширения управления Intune с Intune|
|scriptOutput|String|Выходные данные сценария обнаружения|
|scriptError|String|Ошибка сценария обнаружения|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-shared-manageddevice.md);|Управляемое устройство, на котором выполнен сценарий соответствия устройств требованиям|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "scriptOutput": "String",
  "scriptError": "String"
}
```




