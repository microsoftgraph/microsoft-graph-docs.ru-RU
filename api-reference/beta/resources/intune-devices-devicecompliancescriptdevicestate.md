---
title: тип ресурса deviceComplianceScriptDeviceState
description: Содержит свойства для состояния выполнения устройства скрипта соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1446cb2bc213fb9827f24ff48014950ac5729aa4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612051"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a>тип ресурса deviceComplianceScriptDeviceState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния выполнения устройства скрипта соответствия требованиям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствComplianceScriptDeviceStates](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|[коллекция deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список свойств и связей [объектов deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Get deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Чтение свойств и связей [объекта deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Создание deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Создание нового [объекта deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|
|[Удаление deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|Нет|Удаляет [устройствоComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).|
|[Обновление deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Обновление свойств объекта [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ состояния состояния скрипта устройства устройства. Это свойство доступно только для чтения.|
|detectionState|[runState](../resources/intune-devices-runstate.md)|Состояние обнаружения из последнего выполнения скрипта соответствия требованиям устройства. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения сценария соответствия требованиям устройства|
|expectedStateUpdateDateTime|DateTimeOffset|Следующий период выполнения сценария соответствия требованиям к устройству|
|lastSyncDateTime|DateTimeOffset|Последний раз, когда расширение управления Intune синхронизировали с Intune|
|scriptOutput|String|Выход сценария обнаружения|
|scriptError|String|Ошибка из сценария обнаружения|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемое устройство, на котором выполнен сценарий соответствия требованиям устройства|

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




