---
title: Тип ресурса Девицекомплианцескриптдевицестате
description: Содержит свойства состояния выполнения для сценария соответствия требованиям устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 80177a48e18f1007cd337974d54a016caabd15e4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267686"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a>Тип ресурса Девицекомплианцескриптдевицестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния выполнения для сценария соответствия требованиям устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицекомплианцескриптдевицестатес](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|Коллекция [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список свойств и связей объектов [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Получение Девицекомплианцескриптдевицестате](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Чтение свойств и связей объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Создание Девицекомплианцескриптдевицестате](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Создание нового объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|
|[Удаление Девицекомплианцескриптдевицестате](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|Нет|Удаляет объект [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md).|
|[Обновление Девицекомплианцескриптдевицестате](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Обновление свойств объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния "сценарий соответствия требованиям устройства". Это свойство доступно только для чтения.|
|детектионстате|[рунстате](../resources/intune-shared-runstate.md)|Состояние обнаружения с последнего выполнения скрипта соответствия устройств требованиям. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|ластстатеупдатедатетиме|DateTimeOffset|Последняя метка времени выполнения сценария соответствия требованиям устройства|
|експектедстатеупдатедатетиме|DateTimeOffset|Следующий штамп времени, когда ожидается выполнение сценария соответствия устройства|
|lastSyncDateTime|DateTimeOffset|Время последнего синхронизации расширения управления Intune с Intune|
|скриптаутпут|String|Выходные данные сценария обнаружения|
|скриптеррор|String|Ошибка сценария обнаружения|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md);|Управляемое устройство, на котором выполняется сценарий соответствия устройства|

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




