---
title: Тип ресурса Девицеманажементскриптдевицестате
description: Содержит свойства для состояния запуска на устройстве скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86f3dcfefb80765ff13bb8742d88fdd869072f66
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370048"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Тип ресурса Девицеманажементскриптдевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Ключ объекта состояния устройства сценария управления устройствами.|
|рунстате|[рунстате](../resources/intune-shared-runstate.md)|Состояние последнего запуска скрипта управления устройствами. Возможные значения: `unknown`, `success`, `fail`, `error`, `pending`.|
|ресултмессаже|String|Сведения о выходных данных выполнения.|
|ластстатеупдатедатетиме|DateTimeOffset|Последнее время выполнения скрипта управления устройствами.|
|errorCode|Int32|Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.|
|errorDescription|String|Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.|
|lastSyncDateTime|DateTimeOffset|Последнее время, когда расширение управления Intune будет синхронизироваться с Intune.|
|преремедиатиондетектионскриптаутпут|String|Выходные данные сценария обнаружения перед исправлением.|
|ремедиатионскриптеррор|String|Вывод ошибок сценария исправления.|
|постремедиатиондетектионскриптаутпут|String|Выходные данные сценария обнаружения после исправления.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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
  "errorDescription": "String",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String"
}
```



