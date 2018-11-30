---
title: Управление удостоверениями привилегиями Azure AD
description: Ниже приведен список методы, предоставляемые службой привилегированной управления удостоверениями.
ms.openlocfilehash: ec060c4dc233677f1333e9588e4fb888f8dff9a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074603"
---
# <a name="azure-ad-privileged-identity-management"></a>Управление удостоверениями привилегиями Azure AD

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ниже приведен список методы, предоставляемые службой [Привилегированной управления удостоверениями](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) .

Служба построен на основе OData. Чтобы отфильтровать результаты запроса, используйте стандартные OData ``$filter`` выражения в URI.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) коллекции |Получите коллекцию объектов privilegedOperationEvent. |
|[Получение privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Получите объект privilegedRole.|
|[Список privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) коллекции |Получите коллекцию объектов privilegedRole. |
|[Список назначений ролей](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md) коллекции |Получите privilegedRoleAssignment семейство сайтов для определенной роли. Каждый privilegedRoleAssignment представляет назначения ролей для пользователя.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Активируйте роль, назначенная для инициатора запроса.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Отключение роли, назначенной для инициатора запроса.|
|[Создание privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создайте новый privilegedRoleAssignment (назначение ролей), отправку сообщений в коллекцию privilegedRoleAssignments.|
|[Список privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) коллекции |Получите коллекцию объектов privilegedRoleAssignment. Коллекция содержит все назначения ролей для организации. Каждый privilegedRoleAssignment представляет назначения ролей для пользователя. |
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Получите объект privilegedRoleAssignment с идентификатором указанному назначению. |
|[Удаление privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | Отсутствуют. |Удалите объект privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Сделайте как постоянное назначение ролей. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Сделайте назначения ролей как подходящими. |
|[Мои](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md) коллекции|Получите запрашивающего назначения ролей. |
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Извлечение свойств объекта privilegedRoleSettings. |
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Извлечение объекта privilegedRoleSummary. |
|[Получение privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Получите объект privilegedApproval.|
|[Список privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) коллекции |Получите коллекцию объектов privilegedApproval. |
|[Создание privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Создание объекта privilegedApproval. |
|[Обновление privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Обновление объекта privilegedApproval. |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md) коллекции|Получите запрашивающего запросов на утверждение. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
