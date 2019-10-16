---
title: Тип ресурса Девицехеалсскриптдевицестате
description: Содержит свойства состояния запуска для сценария работоспособности устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9ae4ae7e6f014b52f4049d6663b732680d033d5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539087"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>Тип ресурса Девицехеалсскриптдевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния запуска для сценария работоспособности устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицехеалсскриптдевицестатес](../api/intune-devices-devicehealthscriptdevicestate-list.md)|Коллекция [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список свойств и связей объектов [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Получение Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Чтение свойств и связей объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Создание Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Создание нового объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|
|[Удаление Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|Нет|Удаляет объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md).|
|[Обновление Девицехеалсскриптдевицестате](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Обновление свойств объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния устройства сценария работоспособности. Это свойство доступно только для чтения.|
|детектионстате|[рунстате](../resources/intune-shared-runstate.md)|Состояние обнаружения с последнего выполнения сценария работоспособности устройства. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|ластстатеупдатедатетиме|DateTimeOffset|Последняя метка времени выполнения сценария работоспособности устройства|
|експектедстатеупдатедатетиме|DateTimeOffset|Следующий штамп времени, когда ожидается выполнение сценария работоспособности устройства.|
|lastSyncDateTime|DateTimeOffset|Время последнего синхронизации расширения управления Intune с Intune|
|преремедиатиондетектионскриптаутпут|String|Выходные данные сценария обнаружения перед исправлением|
|преремедиатиондетектионскриптеррор|String|Ошибка сценария обнаружения перед исправлением|
|ремедиатионскриптеррор|String|Вывод ошибок сценария исправления|
|постремедиатиондетектионскриптаутпут|String|Выходные данные сценария обнаружения после исправления|
|постремедиатиондетектионскриптеррор|String|Ошибка сценария обнаружения после исправления|
|ремедиатионстате|[ремедиатионстате](../resources/intune-devices-remediationstate.md)|Состояние исправления с последнего выполнения скрипта работоспособности устройства. Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

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



