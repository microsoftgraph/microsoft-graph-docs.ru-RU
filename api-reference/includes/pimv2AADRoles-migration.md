---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: f956f82fbfb6488f23f7ae155d49c1344ec890e2
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461288"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>Переход на API PIM версии 3 для ролей Azure AD (API управления ролями)

Поддержка интерфейса API PIM для ролей Azure AD прекращена, и он перестал возвращать данные 31 мая 2021 г. Используйте это руководство, чтобы перенести существующие API в новый API [управления ролями](/graph/api/resources/privilegedidentitymanagementv3-overview.md?view=graph-rest-beta&preserve-view=true).

| Operation | API PIM версии 2 | API управления ролями (PIM версии 3) |
| --------- | ------------ | -------------- |
| Перечисление определений ролей | [Перечисление privilegedRoles](/graph/api/privilegedrole-list) | [Перечисление unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| Управление параметрами ролей | [Получение privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[Обновление privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [Управление политиками](/graph/api/policyroot-list-rolemanagementpolicies)
| Создание запросов на назначение ролей | [Создание privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | Используйте [создание unifiedRoleEligibilityScheduleRequest](/graph/api/rbacapplication-post-roleeligibilityschedulerequests) для создания допустимых назначений ролей<br/><br/>Используйте [создание unifiedRoleAssignmentScheduleRequest](/graph/api/rbacapplication-post-roleassignmentschedulerequests) для создания активных назначений ролей |
| Список назначений ролей | [Перечисление privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | Используйте [перечисление unifiedRoleEligibilityScheduleInstances](/graph/api/rbacapplication-list-roleeligibilityscheduleinstances) для получения допустимых назначений ролей<br/><br/>Используйте [перечисление unifiedRoleAssignmentScheduleInstances](/graph/api/rbacapplication-list-roleassignmentscheduleinstances) для получения активных назначений ролей |