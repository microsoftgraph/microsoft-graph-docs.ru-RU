---
title: Privileged Identity Management — ресурсы Azure
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ресурсами Azure.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 50eee822e8386ef7d9e0212f3552432c0f1674ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008868"
---
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management — ресурсы Azure

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно использовать службу [Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) для ресурсов Azure, чтобы настроить рабочий процесс своевременного предоставления доступа для ролей инфраструктуры Azure на уровне групп управления, подписок, групп ресурсов и отдельных ресурсов. Это относится как ко встроенным ролям, таким как "Владелец" и "Участник", так и к настраиваемым ролям RBAC.

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>Основные варианты использования службы PIM и ресурсов Azure с помощью REST API.

| Вариант использования | Ресурс | См. также |
| --- | --- | --- |
| Подключение ресурса (подписок, группы ресурсов, ресурса и т. п.) для управления PIM, создание списка всех управляемых ресурсов, доступных для инициатора запроса, получение отношений управляемого ресурса. | [governanceResource](governanceresource.md) | [Обнаружение ролей и управление ими](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| Список всех ролей ресурса или получение сведений об определенной роли указанного ресурса. | [governanceRoleDefinition](governanceroledefinition.md) |  |
| Получение всех параметров роли для ресурса или обновление параметра роли. | [governanceRoleSetting](governancerolesetting.md) | [Изменение параметров роли](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| Отображение списка и экспорт всех назначений ролей для ресурса. | [governanceRoleAssignment](governanceroleassignment.md) | [Экспорт назначений ролей](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| Создание или удаление допустимого или активного назначения роли, активация и деактивация допустимого назначения, просмотр списка ожидающих запросов, утверждение или отказ ожидающего запроса, отмена вашего собственного ожидающего запроса. | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [Назначение ролей](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[Активация ролей](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[Утверждение запросов](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
