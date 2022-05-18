---
title: Общие сведения об управлении ролями с помощью API управления привилегированными пользователями (PIM)
description: управление привилегированными пользователями (PIM) — это функция Azure AD identity Governance, которая позволяет управлять, контролировать и отслеживать доступ к важным ресурсам в организации.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f254a6ced18f29496ba297c3fe481d75121f9ad7
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461848"
---
# <a name="overview-of-role-management-through-the-privileged-identity-management-pim-api"></a>Общие сведения об управлении ролями с помощью API управления привилегированными пользователями (PIM)

управление привилегированными пользователями (PIM) — это функция Azure AD [identity Governance](/azure/active-directory/governance/identity-governance-overview), которая позволяет управлять, контролировать и отслеживать доступ к важным ресурсам в организации. Этот доступ предоставляется с помощью привилегированных ролей и управления доступом на основе ролей (RBAC) и может быть предоставлен пользователям, группам или субъектам-службам. Ресурсы могут быть в Azure AD, Azure и других облачных службах Майкрософт, таких как Microsoft 365 или Microsoft Intune.

API PIM Graph Майкрософт для управления ролями позволяет управлять привилегированным доступом и ограничивать избыточный доступ. В этой статье представлены возможности управления API PIM в Microsoft Graph.

> [!NOTE]
> Для управления ролями ресурсов Azure используйте API [Azure Resource Manager (ARM) для PIM](/rest/api/authorization/privileged-role-eligibility-rest-sample).

## <a name="pim-api-for-managing-role-assignments"></a>API PIM для управления назначениями ролей

PIM позволяет управлять активными назначениями ролей путем создания постоянных назначений или временных назначений. Используйте тип [ресурса unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) и связанные с ним методы для управления назначениями ролей.

В следующей таблице перечислены сценарии использования PIM для управления назначениями ролей и вызываемого интерфейса API.

|Сценарии  |API  |
|---------|---------|
|Администратор создает и назначает субъекту постоянное назначение ролей.  <br/> Администратор назначает субъекту временную роль   |   [Создание roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Администратор обновляет, обновляет, расширяет или удаляет назначения ролей.     |   [Создание roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Администратор запрашивает все назначения ролей и их сведения     |   [Перечисление roleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)      |
|Администратор запрашивает назначение роли и сведения о ней     |   [Получение unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)      |
|Субъект запрашивает назначения ролей и сведения     |  [unifiedRoleAssignmentScheduleRequest: filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)       |
|Субъект выполняет JIT-активацию с привязкой к времени *для назначения соответствующих* ролей.     |   [Создание roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Субъект отменяет созданный запрос на назначение ролей     |   [unifiedRoleAssignmentScheduleRequest: cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)      |
|Субъект, активированный при назначении подходящей роли, деактивирует его, когда ему больше не нужен доступ.     |   [Создание roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Субъект деактивирует, расширяет или возобновляет назначение собственной роли.     |   [Создание roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |

## <a name="pim-api-for-managing-role-eligibilities"></a>API PIM для управления соответствием требованиям к роли

Вашим субъектам могут не потребоваться постоянные назначения ролей, так как им могут не требоваться привилегии, предоставленные через привилегированную роль, постоянно. В этом случае PIM также позволяет создавать права на роли и назначать их субъектам. При назначении роли субъект активирует роль, когда ему нужно выполнить привилегированные задачи. Активация всегда ограничена временем не более 8 часов. Право на роль также может быть постоянным или временным.

Используйте тип [ресурса unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) и связанные с ним методы для управления допустимостью ролей.

В следующей таблице перечислены сценарии использования PIM для управления допустимости ролей и вызываемого интерфейса API.

|Сценарии  |API  |
|---------|---------|
|Администратор создает и назначает субъекту доступную роль  <br/> Администратор назначает субъекту права на временную роль   |   [Создание roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|Администратор продлевает, обновляет, расширяет или удаляет права на роль     |   [Создание roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|Администратор запрашивает все права на роль и сведения о них.     |   [Перечисление roleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)      |
|Администратор запрашивает право на роль и сведения о ней     |   [Получение unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)      |
|Администратор отменяет созданный запрос на получение прав на роль     |   [unifiedRoleEligibilityScheduleRequest: cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)      |
|Субъект запрашивает разрешения на роль и сведения     |  [unifiedRoleEligibilityScheduleRequest: filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)       |
|Субъект деактивирует, расширяет или обновляет права на собственную роль.     |   [Создание roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |


## <a name="role-settings-and-pim"></a>Параметры роли и PIM

Каждая Azure AD определяет параметры или правила. Такие параметры включают в себя необходимость многофакторной проверки подлинности (MFA), обоснование или утверждение для активации подходящей роли или возможность создания постоянных назначений или прав субъектов на роль. Эти параметры, связанные с ролями, определяют параметры, которые можно применять при создании назначений ролей и назначений ролей, а также управлении ими с помощью PIM. В Microsoft Graph управление этими параметрами ролей осуществляется с помощью [unifiedRoleManagementPolicy](unifiedrolemanagementpolicy.md), типов ресурсов [unifiedRoleManagementPolicyAssignment](unifiedrolemanagementpolicyassignment.md) и связанных с ними методов.

Например, предположим, что по умолчанию роль не допускает постоянных активных назначений и определяет не более 15 дней для активных назначений. При попытке создать объект [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) `400 Bad Request` без даты окончания срока действия возвращается код ответа на нарушение правила истечения срока действия.

В следующей таблице перечислены сценарии использования PIM для Azure AD параметров ролей или правил и вызываемого интерфейса API.

|Сценарии  |API  |
|---------|---------|
|Получение политик управления ролами и связанных правил или параметров   |   [Перечисление unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)      |
|Получение политики управления ролем и связанных с ней правил или параметров |   [Получение unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)      |
|Получение правил или параметров, определенных для политики управления ролем | [Список правил](../api/unifiedrolemanagementpolicy-list-rules.md)       |
|Получение правила или параметров, определенных для политики управления ролем |  [Получение unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)      |
|Обновление правила или параметра, определенного для политики управления ролем|[Обновление unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|
|Получение сведений о всех назначениях политик управления ролями, включая политики, правила или параметры, связанные с Azure AD ролей. |  [Перечисление объектов unifiedRoleManagementPolicyAssignment](../api/policyroot-list-rolemanagementpolicyassignments.md)      |
|Получение сведений о назначении политики управления ролем, включая политику, правила или параметры, связанные с Azure AD роли |   [Получение объекта unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)     |

Дополнительные сведения о параметрах ролей см. в Azure AD [параметров роли в управление привилегированными пользователями](/azure/active-directory/privileged-identity-management/pim-how-to-change-default-settings).

## <a name="pim-and-identity-security-with-zero-trust"></a>PIM и безопасность удостоверений с помощью функции "Никому не доверяй"

API PIM позволяют организациям применять подход "Никому не доверяй" для защиты удостоверений в своей организации. Дополнительные сведения об нулевом доверии см. в статье ["Защита удостоверений с помощью модели "Никому не доверяй"](/security/zero-trust/deploy/identity).

## <a name="permissions-and-privileges"></a>Разрешения и привилегии

Чтобы вызвать API [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) и [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) с действиями администратора, вызывающий пользователь должен:
+ Роль *глобального администратора* или *администратора привилегированных* ролей
+ Предоставьте одно из следующих разрешений:
  + RoleAssignmentSchedule.ReadWrite.Directory
  + RoleEligibilitySchedule.ReadWrite.Directory
  + RoleManagement.ReadWrite.Directory

Субъекту также должны быть назначены соответствующие разрешения для получения назначений ролей и разрешений, или вызвать API [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) и [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) с действиями пользователя.

Дополнительные сведения о разрешениях на вызов API PIM см. в Graph microsoft [Graph: разрешения на управление ролами](/graph/permissions-reference#role-management-permissions).

## <a name="licensing"></a>Лицензирование

Для API PIM требуется Azure AD Premium P2 лицензии. Дополнительные сведения см[. в разделе "Требования к лицензии для использования управление привилегированными пользователями](/azure/active-directory/privileged-identity-management/subscription-requirements)".

## <a name="see-also"></a>Дополнительные ресурсы

+ [Что такое Azure AD Privileged Identity Management?](/azure/active-directory/privileged-identity-management/pim-configure)
+ [Руководство. Использование API управление привилегированными пользователями (PIM) для назначения Azure AD ролей](/graph/tutorial-assign-azureadroles)
+ Вы также можете настроить проверки доступа для назначений ролей и прав доступа, управляемых с помощью PIM. Дополнительные сведения см. в руководстве по использованию [API управление привилегированными пользователями (PIM) для назначения Azure AD ролей](/graph/tutorial-assign-azureadroles).