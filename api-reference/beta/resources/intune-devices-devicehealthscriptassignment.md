---
title: Тип ресурса Девицехеалсскриптассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e1ed01161b6b7b9002b3db9a0473c058db3185e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443210"
---
# <a name="devicehealthscriptassignment-resource-type"></a>Тип ресурса Девицехеалсскриптассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицехеалсскриптассигнментс](../api/intune-devices-devicehealthscriptassignment-list.md)|Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)|Список свойств и связей объектов [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Получение Девицехеалсскриптассигнмент](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Чтение свойств и связей объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Создание Девицехеалсскриптассигнмент](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Создание нового объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .|
|[Удаление Девицехеалсскриптассигнмент](../api/intune-devices-devicehealthscriptassignment-delete.md)|Нет|Удаляет объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md).|
|[Обновление Девицехеалсскриптассигнмент](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Обновление свойств объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения сценария работоспособности устройства. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Группа Azure Active Directory, на которую мы нацелены на скрипт|
|рунремедиатионскрипт|Логическое|Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Расписание запуска сценария для целевой группы|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



