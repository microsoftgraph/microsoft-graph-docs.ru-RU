---
title: Privileged Identity Management — ресурсы Azure
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ресурсами Azure.
localization_priority: Priority
author: shauliu1
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 48d0a4ceebee14a504b90433da21ce1f28392393
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453830"
---
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management — ресурсы Azure

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно использовать службу [Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) для ресурсов Azure, чтобы настроить рабочий процесс своевременного предоставления доступа для ролей инфраструктуры Azure на уровне групп управления, подписок, групп ресурсов и отдельных ресурсов. Это относится как ко встроенным ролям, таким как "Владелец" и "Участник", так и к настраиваемым ролям RBAC.

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>Основные варианты использования службы PIM и ресурсов Azure с помощью REST API.

| Вариант использования | Ресурс | См. также |
| --- | --- | --- |
| Подключение ресурса (подписок, группы ресурсов, ресурса и т. п.) для управления PIM, создание списка всех управляемых ресурсов, доступных для инициатора запроса, получение отношений управляемого ресурса. | [governanceResource](governanceresource.md) | [Обнаружение ролей и управление ими](/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| Список всех ролей ресурса или получение сведений об определенной роли указанного ресурса. | [governanceRoleDefinition](governanceroledefinition.md) |  |
| Получение всех параметров роли для ресурса или обновление параметра роли. | [governanceRoleSetting](governancerolesetting.md) | [Изменение параметров роли](/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| Отображение списка и экспорт всех назначений ролей для ресурса. | [governanceRoleAssignment](governanceroleassignment.md) | [Экспорт назначений ролей](/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| Создание или удаление допустимого или активного назначения роли, активация и деактивация допустимого назначения, просмотр списка ожидающих запросов, утверждение или отказ ожидающего запроса, отмена вашего собственного ожидающего запроса. | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [Назначение ролей](/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[Активация ролей](/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[Утверждение запросов](/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
