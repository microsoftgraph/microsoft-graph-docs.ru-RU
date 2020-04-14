---
title: Тип ресурса Ролескопетагаутоассигнмент
description: Содержит свойства для автоматического назначения тега области роли группе, которая будет применена к устройствам.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77d563f9ef99f9e8d6cce9577ec60a4c289f4a8f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356780"
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



