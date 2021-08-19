---
title: тип ресурса deviceHealthScriptDeviceState
description: Содержит свойства для состояния запуска устройства скрипта здоровья устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e80f47a2daa68bffb8d90c536bf066ad0b1a303d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256082"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>тип ресурса deviceHealthScriptDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска устройства скрипта здоровья устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceHealthScriptDeviceStates](../api/intune-devices-devicehealthscriptdevicestate-list.md)|[коллекция deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список свойств и связей [объектов deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Get deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Чтение свойств и связей [объекта deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Создание deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Создание нового [объекта deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|
|[Удаление deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Нет|Удаляет [устройствоHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).|
|[Обновление устройстваHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Обновление свойств объекта [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ состояния состояния скрипта устройства для устройства. Это свойство доступно только для чтения.|
|detectionState|[runState](../resources/intune-devices-runstate.md)|Состояние обнаружения из последнего выполнения скрипта для здоровья устройств. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения скрипта для здоровья устройств|
|expectedStateUpdateDateTime|DateTimeOffset|Следующий период, когда ожидается выполнение сценария состояния устройства|
|lastSyncDateTime|DateTimeOffset|Последний раз, когда расширение управления Intune синхронизировали с Intune|
|preRemediationDetectionScriptOutput|String|Выход сценария обнаружения перед исправлением|
|preRemediationDetectionScriptError|String|Ошибка из сценария обнаружения перед исправлением|
|remediationScriptError|Строка|Выход ошибки сценария восстановления|
|postRemediationDetectionScriptOutput|Строка|Вывод скрипта обнаружения после устранения|
|postRemediationDetectionScriptError|Строка|Ошибка из сценария обнаружения после устранения|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Состояние исправлений из последнего выполнения скрипта для здоровья устройств. Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|
|assignmentFilterIds|Коллекция String|Список ids фильтра назначения, используемых для оценки применимости скрипта для здоровья|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемое устройство, на котором выполнялся сценарий состояния устройства|

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
  "remediationState": "String",
  "assignmentFilterIds": [
    "String"
  ]
}
```




