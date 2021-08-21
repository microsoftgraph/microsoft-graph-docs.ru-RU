---
title: Тип ресурса rbacApplication
description: Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e6157355fe71d0643c9fff354a4932fc020a9ffd
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454187"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса rbacApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC. В настоящее время каталог и управление правами — это единственные поддерживаемые приложения RBAC.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignments. |
| [Список объектов roleAssignment](../api/rbacapplication-list-roleassignments.md) | [коллекция unifiedRoleAssignment](unifiedroleassignment.md) | Получите коллекцию объектов unifiedRoleAssignment. Только определенные экземпляры можно запрашивать, фильтруя на roleDefitionId или principalId. |
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Получите коллекцию объектов unifiedRoleDefinition. |
| [roleSchedules](../api/rbacapplication-roleschedules.md) | [коллекция unifiedRoleScheduleBase](unifiedroleschedulebase.md) | Функция получения коллекции объектов unifiedRoleScheduleBase. |
| [roleScheduleInstances](../api/rbacapplication-rolescheduleinstances.md) | [коллекция unifiedRoleScheduleInstanceBase](unifiedrolescheduleinstancebase.md) | Функция получения коллекции объектов unifiedRoleScheduleInstanceBase.  |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleDefinitions|[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, присвоенные ролям. |
|roleAssignmentApprovals|[коллекция утверждений](../resources/approval.md)| Решения, связанные с утверждением назначения ролей.|
|roleAssignmentScheduleInstances|[коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)| Экземпляры для активных назначений ролей через Azure AD управление привилегированными пользователями.  |
|roleAssignmentScheduleRequests|[коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Запросы на активные назначения ролей через Azure AD управление привилегированными пользователями. |
|roleAssignmentSchedules|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md)| Расписание назначений активных ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilityScheduleInstances|[коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md)| Примеры подходящих назначений ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilityScheduleRequests|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md)| Запросы на подходящие назначения ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilitySchedules|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md)| Расписание назначений подходящих ролей через Azure AD управление привилегированными пользователями. |



## <a name="json-representation"></a>Представление JSON

Нет

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


