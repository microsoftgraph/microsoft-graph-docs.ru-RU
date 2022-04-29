---
title: Тип ресурса rbacApplication
description: Контейнер для определений ролей и назначений ролей для Microsoft 365 управления доступом на основе ролей (RBAC)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9949ea7f219cee7e92f2c1406fe140469d67ad8c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133785"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса rbacApplication

Пространство имен: microsoft.graph

Контейнер управления ролами для унифицированных определений ролей и назначений ролей для Microsoft 365 управления доступом на основе ролей (RBAC). Назначения ролей поддерживают только один субъект и одну область. В **настоящее время** **каталог и entitlementManagement** поддерживаются двумя поставщиками RBAC.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|[Коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleAssignmentScheduleInstances|[Коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)| Экземпляры для активных назначений ролей.  |
|roleAssignmentScheduleRequests|[Коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Запросы на активные назначения ролей субъектам через PIM. |
|roleAssignmentSchedules|[Коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Расписания для активных операций назначения ролей.|
|roleDefinitions|[Коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, назначенные ролям. |
|roleEligibilityScheduleInstances|[Коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Экземпляры для запросов на получение прав на роль.|
|roleEligibilityScheduleRequests|[Коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)| Запросы на получение прав на роль для субъектов через PIM.|
|roleEligibilitySchedules|[Коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Расписания для операций, применимости к роли. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rbacApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "String (identifier)"
}
```
