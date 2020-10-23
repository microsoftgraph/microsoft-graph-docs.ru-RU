---
title: Тип ресурса Девицехеалсскриптдевицестате
description: Содержит свойства состояния запуска для сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5413e00e299633313e6f823dc5b60bf13df5ce56
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697730"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>Тип ресурса Девицехеалсскриптдевицестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния запуска для сценария работоспособности устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицехеалсскриптдевицестатес](../api/intune-devices-devicehealthscriptdevicestate-list.md)|Коллекция [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список свойств и связей объектов [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Получение Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Чтение свойств и связей объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Создание Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Создание нового объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Удаление Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Нет|Удаляет объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md).|
|[Обновление Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Обновление свойств объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта состояния устройства сценария работоспособности. Это свойство доступно только для чтения.|
|детектионстате|[рунстате](../resources/intune-shared-runstate.md)|Состояние обнаружения с последнего выполнения сценария работоспособности устройства. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|ластстатеупдатедатетиме|DateTimeOffset|Последняя метка времени выполнения сценария работоспособности устройства|
|експектедстатеупдатедатетиме|DateTimeOffset|Следующий штамп времени, когда ожидается выполнение сценария работоспособности устройства.|
|lastSyncDateTime|DateTimeOffset|Время последнего синхронизации расширения управления Intune с Intune|
|преремедиатиондетектионскриптаутпут|Строка|Выходные данные сценария обнаружения перед исправлением|
|преремедиатиондетектионскриптеррор|Строка|Ошибка сценария обнаружения перед исправлением|
|ремедиатионскриптеррор|Строка|Вывод ошибок сценария исправления|
|постремедиатиондетектионскриптаутпут|Строка|Выходные данные сценария обнаружения после исправления|
|постремедиатиондетектионскриптеррор|Строка|Ошибка сценария обнаружения после исправления|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Состояние исправления с последнего выполнения скрипта работоспособности устройства. Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемое устройство, на котором выполняется сценарий работоспособности устройства|

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





