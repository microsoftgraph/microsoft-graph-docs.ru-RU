---
title: Тип ресурса unifiedRoleAssignmentSchedule
description: Представляет расписание для назначения активной роли в клиенте.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7294918800c68857ca11ac41a7baf8fab7e4da5e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134389"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>Тип ресурса unifiedRoleAssignmentSchedule

Пространство имен: microsoft.graph

Представляет расписание для активного назначения ролей в клиенте и используется для создания экземпляра [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). Активное назначение может быть выполнено через [назначения PIM](../api/rbacapplication-post-roleassignmentschedulerequests.md) и запросы на активацию или непосредственно через [API назначений ролей](../resources/unifiedroleassignment.md).

Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleAssignmentSchedule](../api/rbacapplication-list-roleassignmentschedules.md)|[Коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получение расписаний для активных операций назначения ролей.|
|[Получение unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получение расписания для операции назначения активной роли.|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получение расписаний для активных операций назначения ролей, для которых вошед в систему пользователь является субъектом.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к конкретному приложению, если назначение предназначено для приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. `$filter` Поддерживает (`eq`и `ne`по `null` значениям). Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|assignmentType|String|Тип назначения, которое может быть или `Assigned` `Activated`. Поддерживает `$filter` (`eq`, `ne`).|
|createdDateTime|DateTimeOffset|При создании расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|String|Идентификатор объекта **unifiedRoleAssignmentScheduleRequest** , с помощью которого было создано это расписание. Допускается значение null. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. `$filter` Поддерживает (`eq`и `ne`по `null` значениям). Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|String|Уникальный идентификатор объекта **unifiedRoleAssignmentScheduleRequest** . Поддерживает `$filter` (`eq`). Наследуется от [сущности](../resources/entity.md).|
|memberType|String|Способ наследования назначений. Это может быть либо `Inherited`, `Direct`, либо `Group`. Это также может означать, может ли **объект unifiedRoleAssignmentSchedule** управляться вызывающим объектом. Поддерживает `$filter` (`eq`, `ne`).|
|modifiedDateTime|DateTimeOffset|Время последнего изменения расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String|Идентификатор субъекта, которым было предоставлено назначение роли. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Поддерживает `$filter` (`eq`, `ne`).|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Поддерживает `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период назначения роли. Он может представлять одно или несколько повторений.|
|status|String|Состояние объекта **unifiedRoleAssignmentScheduleRequest** . Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Возможные значения: `Canceled`, , `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`и `Revoked``ScheduleCreated`. Значение null не допускается. Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если запрос от допустимого администратора для активации роли, этот параметр отобразит связанное допустимое назначение для этой активации. В противном случае это .`null` Поддерживает `$expand`.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если назначение предназначено для приложения. Допускается значение null. Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Только для чтения. Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли через запрос. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** . Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "assignmentType": "String",
  "memberType": "String"
}
```

