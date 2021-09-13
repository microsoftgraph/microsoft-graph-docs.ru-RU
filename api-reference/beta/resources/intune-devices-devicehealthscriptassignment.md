---
title: тип ресурса deviceHealthScriptAssignment
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5ae4954314224db4bd65278e95ed8f0e7a8ec9b8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017389"
---
# <a name="devicehealthscriptassignment-resource-type"></a>тип ресурса deviceHealthScriptAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствHealthScriptAssignments](../api/intune-devices-devicehealthscriptassignment-list.md)|[коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Список свойств и связей [объектов deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Get deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Чтение свойств и связей [объекта deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Создание deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Создайте новый [объект deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|
|[Удаление deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-delete.md)|Нет|Удаляет [устройствоHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).|
|[Обновление устройстваHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Обновление свойств объекта [deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения скрипта для скрипта устройства. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Группа Azure Active Directory, на которые мы нацелим сценарий|
|runRemediationScript|Boolean|Определите, нужно ли запускать только сценарий обнаружения или запускать сценарий обнаружения и сценарий восстановления.|
|runSchedule|[deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|Расписание запуска скрипта для целевой группы|

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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 1024,
    "useUtc": true,
    "time": "String (time of day)"
  }
}
```



