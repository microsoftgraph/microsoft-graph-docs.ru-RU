---
title: Тип ресурса roleScopeTagAutoAssignment
description: Содержит свойства автоматического присвоения тега области ролей группе, которая будет применяться к устройствам.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84bcaccc1206bb71e74e197bc7932a7a12ff6361
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806007"
---
# <a name="rolescopetagautoassignment-resource-type"></a>Тип ресурса roleScopeTagAutoAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства автоматического присвоения тега области ролей группе, которая будет применяться к устройствам.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|[коллекция roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Список свойств и связей объектов [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Get roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Чтение свойств и связей [объекта roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Создание roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Создайте новый [объект roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Удаление roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|Нет|Удаляет [рольScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).|
|[Update roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Обновление свойств объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель автоматического назначения для определенного тега области ролей.|

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



