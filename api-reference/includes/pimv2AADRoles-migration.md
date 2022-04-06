---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: 9e636421a8fa64f14b331c7f774e8f252698a2c8
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509240"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>Переход на API PIM версии 3 для ролей Azure AD (API управления ролями)

Поддержка интерфейса API PIM для ролей Azure AD прекращена, и он перестал возвращать данные 31 мая 2021 г. Используйте это руководство, чтобы перенести существующие API в новый API [управления ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true).

| Operation | API PIM версии 2 | API управления ролями (PIM версии 3) |
| --------- | ------------ | -------------- |
| Перечисление определений ролей | [Перечисление privilegedRoles](/graph/api/privilegedrole-list) | [Перечисление unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| Управление параметрами ролей | [Получение privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[Обновление privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [Управление политиками](/graph/api/unifiedrolemanagementpolicy-list)
| Создание запросов на назначение ролей | [Создание privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | Используйте [создание unifiedRoleEligibilityScheduleRequest](/graph/api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests) для создания допустимых назначений ролей<br/><br/>Используйте [создание unifiedRoleAssignmentScheduleRequest](/graph/api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests) для создания активных назначений ролей |
| Список назначений ролей | [Перечисление privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | Используйте [перечисление unifiedRoleEligibilityScheduleInstances](/graph/api/unifiedroleeligibilityscheduleinstance-list) для получения допустимых назначений ролей<br/><br/>Используйте [перечисление unifiedRoleAssignmentScheduleInstances](/graph/api/unifiedroleassignmentscheduleinstance-list) для получения активных назначений ролей |