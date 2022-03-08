---
title: Тип ресурса rbacApplication
description: Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 74b6fe87456108ba66bf4db4363434cc45133ce9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336769"
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
| [Список transitiveRoleAssignments](../api/rbacapplication-list-transitiveroleassignments.md) | [коллекция unifiedRoleAssignment](unifiedroleassignment.md) | Получите прямые и транзитные унифицированные унифицированные функции, назначенные определенному принципу. Необходимо указать principalId. |
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Получите коллекцию объектов unifiedRoleDefinition. |
| [roleSchedules](../api/rbacapplication-roleschedules.md) | [коллекция unifiedRoleScheduleBase](unifiedroleschedulebase.md) | Функция получения коллекции объектов unifiedRoleScheduleBase. |
| [roleScheduleInstances](../api/rbacapplication-rolescheduleinstances.md) | [коллекция unifiedRoleScheduleInstanceBase](unifiedrolescheduleinstancebase.md) | Функция получения коллекции объектов unifiedRoleScheduleInstanceBase.  |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|resourceNamespaces|[коллекция unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Ресурс, представляючий коллекцию связанных действий.|
|roleAssignments|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleDefinitions|[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, присвоенные ролям. |
|roleAssignmentApprovals|[коллекция утверждений](../resources/approval.md)| Решения, связанные с утверждением назначения ролей.|
|roleAssignmentScheduleInstances|[коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)| Экземпляры для активных назначений ролей через Azure AD управление привилегированными пользователями.  |
|roleAssignmentScheduleRequests|[коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Запросы на активные назначения ролей через Azure AD управление привилегированными пользователями. |
|roleAssignmentSchedules|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md)| Расписание назначений активных ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilityScheduleInstances|[коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md)| Примеры подходящих назначений ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilityScheduleRequests|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md)| Запросы на подходящие назначения ролей через Azure AD управление привилегированными пользователями. |
|roleEligibilitySchedules|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md)| Расписание назначений подходящих ролей через Azure AD управление привилегированными пользователями. |
|transitiveRoleAssignments|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа к пользователям или группам, которые являются транзитными. |


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


