---
title: Тип ресурса deviceHealthScriptDeviceState
description: Содержит свойства состояния запуска устройства для сценария состояния устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5804a3f648ef60d55cfe99008ef790afdef55888
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272284"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>Тип ресурса deviceHealthScriptDeviceState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния запуска устройства для сценария состояния устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceHealthScriptDeviceStates](../api/intune-devices-devicehealthscriptdevicestate-list.md)|[Коллекция deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список свойств и связей объектов [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Get deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Чтение свойств и связей объекта [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Создание deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Создание объекта [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Удаление deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Нет|Удаляет [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Обновление deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Обновление свойств объекта [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния устройства скрипта состояния устройства. Это свойство доступно только для чтения.|
|detectionState|[runState](../resources/intune-shared-runstate.md)|Состояние обнаружения из последнего выполнения скрипта для определения состояния устройства. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|Последняя временная запаздывка выполнения скрипта о состоянии устройства|
|expectedStateUpdateDateTime|DateTimeOffset|Следующая временная запаздывка ожидаемого выполнения скрипта о состоянии устройства|
|lastSyncDateTime|DateTimeOffset|Время последней синхронизации расширения управления Intune с Intune|
|preRemediationDetectionScriptOutput|String|Вывод скрипта обнаружения перед исправлением|
|preRemediationDetectionScriptError|String|Ошибка скрипта обнаружения перед исправлением|
|remediationScriptError|String|Выходные данные об ошибках сценария устранения ошибок|
|postRemediationDetectionScriptOutput|String|Вывод скрипта обнаружения после устранения|
|postRemediationDetectionScriptError|String|Ошибка сценария обнаружения после устранения ошибок|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Состояние устранения из последнего выполнения скрипта для системы. Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-shared-manageddevice.md);|Управляемое устройство, на котором выполнен сценарий состояния устройства|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```




