---
title: Тип ресурса Девицехеалсскриптассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6704afe5e105491e2be35bda1e68dd446f3c88
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088303"
---
# <a name="devicehealthscriptassignment-resource-type"></a>Тип ресурса Девицехеалсскриптассигнмент

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
|рунремедиатионскрипт|Логический|Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.|
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



