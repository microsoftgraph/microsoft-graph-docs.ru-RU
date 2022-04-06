---
author: carolinetempleton
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: c17741c368295201dd626df91de161cf318efc1b
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477855"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-the-azure-resource-manager-arm-pim-api-for-azure-resource-roles"></a>Переход на API PIM Azure Resource Manager (ARM) для ролей ресурсов Azure

API PIM версии 3 для управления ресурсами Azure теперь доступен через REST API Azure Resource Manager (ARM). Используйте это руководство для переноса существующих API в новые [API Azure Resource Manager (ARM)](/rest/api/authorization/privileged-role-eligibility-rest-sample).

В следующей таблице описывается, как новые API ARM сопоставляются с существующими API.

| Operation | API Microsoft Graph (PIM версии 2) | API ARM (PIM версии 3) |
| --------- | ------------ | -------------- |
| Регистрация ресурса | [Регистрация](/graph/api/governanceresource-register) | ARM не требует, чтобы ресурсы были явно зарегистрированы или подключены для управления ими. Вы можете выполнять операции напрямую с помощью области ресурсов. |
| Перечисление определений ролей | [Перечисление определений ролей](/graph/api/governanceroledefinition-list) | [Определения ролей — список](/rest/api/authorization/role-definitions/list) |
| Создание запросов на назначение ролей | [Создание governanceRoleAssignmentRequest](/graph/api/governanceroleassignmentrequest-post) | Используйте [запросы на планирование допустимости ролей — создание](/rest/api/authorization/role-eligibility-schedule-requests/create) для создания допустимых назначений ролей<br/><br/>Используйте [запросы на планирование назначений ролей — создание](/rest/api/authorization/role-assignment-schedule-requests/create) для создания активных назначений ролей |
| Список назначений ролей | [Перечисление governanceRoleAssignments](/graph/api/governanceroleassignment-list) | Используйте [экземпляры планирования допустимости ролей — перечисление](/rest/api/authorization/role-eligibility-schedule-instances/list-for-scope) для получения допустимых назначений ролей<br/><br/>Используйте [экземпляры планирования назначений ролей — перечисление](/rest/api/authorization/role-assignment-schedule-instances/list-for-scope) для получения активных назначений ролей |
| Управление параметрами ролей | [Перечисление governanceRoleSettings](/graph/api/governancerolesetting-list)<br/>[Обновление governanceRoleSetting](/graph/api/governancerolesetting-update) | [Управление политиками с помощью ARM](/rest/api/authorization/privileged-role-policy-rest-sample)