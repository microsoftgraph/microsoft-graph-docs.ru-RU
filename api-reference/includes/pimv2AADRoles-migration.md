---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: ba8ba53c60d37d55cffba7b3f9626832bbf2f1cc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441713"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>Переход на API PIM версии 3 для ролей Azure AD (API управления ролями)

Поддержка интерфейса API PIM для ролей Azure AD прекращена, и он перестал возвращать данные 31 мая 2021 г. Используйте это руководство, чтобы перенести существующие API в новый [API управления ролями для управления привилегированными удостоверениями](/graph/api/resources/privilegedidentitymanagementv3-overview).

| Operation | API PIM версии 2 | API управления ролями (PIM версии 3) |
| --------- | ------------ | -------------- |
| Перечисление определений ролей | [Перечисление privilegedRoles](/graph/api/privilegedrole-list) | [Перечисление unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| Управление параметрами ролей | [Получение privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[Обновление privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [Управление политиками](/graph/api/policyroot-list-rolemanagementpolicies)
| Создание запросов на назначение ролей | [Создание privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | Используйте [создание unifiedRoleEligibilityScheduleRequest](/graph/api/rbacapplication-post-roleeligibilityschedulerequests) для создания допустимых назначений ролей<br/><br/>Используйте [создание unifiedRoleAssignmentScheduleRequest](/graph/api/rbacapplication-post-roleassignmentschedulerequests) для создания активных назначений ролей |
| Список назначений ролей | [Перечисление privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | Используйте [перечисление unifiedRoleEligibilityScheduleInstances](/graph/api/rbacapplication-list-roleeligibilityscheduleinstances) для получения допустимых назначений ролей<br/><br/>Используйте [перечисление unifiedRoleAssignmentScheduleInstances](/graph/api/rbacapplication-list-roleassignmentscheduleinstances) для получения активных назначений ролей |
