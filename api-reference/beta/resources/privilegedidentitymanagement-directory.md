---
title: Privileged Identity Management — Azure AD
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory.
ms.localizationpriority: high
author: carolinetempleton
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 900038e9c68517ac42ade68218b55d7cc52450f9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688782"
---
# <a name="privileged-identity-management---azure-ad-deprecated"></a>Privileged Identity Management — Azure AD (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Следующие методы предоставляются службой PIM для ролей Azure AD. Служба создана на основе OData. Чтобы отфильтровать результаты запросов, используйте стандартные выражения OData `$filter` в URI.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | Коллекция [privilegedOperationEvent](privilegedoperationevent.md) |Получение коллекции объектов privilegedOperationEvent. |
|[Получение privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Получение объекта privilegedRole.|
|[Перечисление privilegedRole](../api/privilegedrole-list.md) | Коллекция [privilegedRole](privilegedrole.md) |Получение коллекции объектов privilegedRole. |
|[Перечисление назначений ролей](../api/privilegedrole-list-assignments.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md) |Получение коллекции privilegedRoleAssignment для конкретной роли. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Активация роли, назначенной запрашивающей стороне.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Деактивация роли, назначенной запрашивающей стороне.|
|[Создание privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создание нового объекта privilegedRoleAssignment (назначение роли) путем публикации в коллекции privilegedRoleAssignments.|
|[Перечисление privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md) |Получение коллекции объектов privilegedRoleAssignment. Коллекция содержит все назначения ролей для организации. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю. |
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Получение объекта privilegedRoleAssignment с указанным идентификатором назначения. |
|[Удаление privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | Нет. |Удаление объекта privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Выполнение назначения ролей как бессрочного. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Выполнение назначения ролей как соответствующего требованиям. |
|[my](../api/privilegedroleassignment-my.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получение назначений ролей запрашивающей стороны. |
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Получение свойств объекта privilegedRoleSettings. |
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Получение объекта privilegedRoleSummary. |
|[Получение privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Получение объекта privilegedApproval.|
|[Перечисление privilegedApproval](../api/privilegedapproval-list.md) | Коллекция [privilegedApproval](privilegedapproval.md) |Получение коллекции объектов privilegedApproval. |
|[Создание privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Создание объекта privilegedApproval. |
|[Обновление privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Обновление объекта privilegedApproval. |
|[myrequests](../api/privilegedapproval-myrequests.md) | Коллекция [privilegedApproval](privilegedapproval.md)|Получение запросов утверждения запрашивающей стороны. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
