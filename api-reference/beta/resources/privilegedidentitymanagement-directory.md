---
title: Privileged Identity Management — Azure AD
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 3bc7f9cdb9c998e3140148eee274a2831f3a34c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521546"
---
# <a name="privileged-identity-management---azure-ad"></a>Privileged Identity Management — Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> Интерфейс API [службы Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) для управления ролями Azure AD будет изменяться с июня по ноябрь 2019 года для соответствия пространству имен и соглашению для [интерфейсов API ресурсов Azure](privilegedidentitymanagement-resources.md). Служба Azure AD PIM станет ресурсом в соответствии с соглашением о ресурсах Azure. Если это изменение непосредственно повлияет на ваш клиент, заполните [форму изменения интерфейса API Graph для Azure AD PIM](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u), чтобы получить дополнительные сведения, поддержку и возможность запланировать время для этого изменения API.

Ниже приведен список методов, предоставляемых службой PIM для ролей Azure AD. Служба создана на основе OData. Чтобы отфильтровать результаты запросов, используйте стандартные выражения OData ``$filter`` в URI.

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
