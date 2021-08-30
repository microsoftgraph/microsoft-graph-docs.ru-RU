---
title: Privileged Identity Management — Azure AD
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory.
ms.localizationpriority: high
author: shauliu1
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 045656549e00dce0a97586cfe02564e8271d70ed
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695261"
---
# <a name="privileged-identity-management---azure-ad"></a>Privileged Identity Management — Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> Поддержка API для управления ролями Azure AD прекращается в большинстве клиентов, кроме нескольких, использующих более раннюю версию управления привилегированными пользователями (PIM). Дополнительные сведения о версиях PIM см. в разделе [Определение версии PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim). Если вы используете новую версию и у вас возникает ошибка **TenantEnabledInAadRoleMigration**, вы можете подождать появления нового API для функций PIM в API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) для ролей Azure AD или использовать API [ресурса Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) для ролей Azure AD. Чтобы использовать API **ресурса Azure**, замените `azureResources` на `aadRoles` для `provider_id` и используйте свой идентификатор клиента для `resource_id`. Мы рекомендуем дождаться нового API. После появления нового API вы сможете продолжать использование API **ресурса Azure**. Любые новые функции, которые будут доступны на портале Azure, также будут доступны только через новый API-интерфейс.

Следующие методы предоставляются службой PIM для ролей Azure AD. Служба создана на основе OData. Чтобы отфильтровать результаты запросов, используйте стандартные выражения OData ``$filter`` в URI.

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
