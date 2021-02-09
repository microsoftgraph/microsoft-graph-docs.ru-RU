---
title: Тип ресурса roleScopeTagAutoAssignment
description: Содержит свойства автоматического назначения тега области роли группе, применяемой к устройствам.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d270b09a980ad90dd18e590bc3d6b44342dc9984
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157521"
---
# <a name="rolescopetagautoassignment-resource-type"></a>Тип ресурса roleScopeTagAutoAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства автоматического назначения тега области роли группе, применяемой к устройствам.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|[Коллекция roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Список свойств и связей объектов [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Get roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Чтение свойств и связей объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Создание roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Создание объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Удаление roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|Нет|Удаляет [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Обновление roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Обновление свойств объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевой объект автоматического назначения для определенного тега области роли.|

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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




