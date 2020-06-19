---
title: Тип ресурса Ролескопетагаутоассигнмент
description: Содержит свойства для автоматического назначения тега области роли группе, которая будет применена к устройствам.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d136ed1f67578b22b36be2e34ff2ada81b7cbf9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793628"
---
# <a name="rolescopetagautoassignment-resource-type"></a>Тип ресурса Ролескопетагаутоассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для автоматического назначения тега области роли группе, которая будет применена к устройствам.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ролескопетагаутоассигнментс](../api/intune-rbac-rolescopetagautoassignment-list.md)|Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)|Список свойств и связей объектов [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Получение Ролескопетагаутоассигнмент](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Чтение свойств и связей объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Создание Ролескопетагаутоассигнмент](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Создание нового объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Удаление Ролескопетагаутоассигнмент](../api/intune-rbac-rolescopetagautoassignment-delete.md)|Нет|Удаляет объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md).|
|[Обновление Ролескопетагаутоассигнмент](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Обновление свойств объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевой объект автоматического назначения для определенного тега области применения роли.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



