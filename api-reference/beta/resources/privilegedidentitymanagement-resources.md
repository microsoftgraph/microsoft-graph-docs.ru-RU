---
title: Privileged Identity Management — ресурсы Azure
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ресурсами Azure.
ms.localizationpriority: high
author: carolinetempleton
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: ec3c67b8ffcb35a223f1491a40bab55e92563c28
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "64477932"
---
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management — ресурсы Azure

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Можно использовать службу [Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) для ресурсов Azure, чтобы настроить рабочий процесс своевременного предоставления доступа для ролей инфраструктуры Azure на уровне групп управления, подписок, групп ресурсов и отдельных ресурсов. Это относится как ко встроенным ролям, таким как "Владелец" и "Участник", так и к настраиваемым ролям RBAC.

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>Основные варианты использования службы PIM и ресурсов Azure с помощью REST API.

| Вариант использования | Ресурс | См. также |
| --- | --- | --- |
| Подключение ресурса (подписок, группы ресурсов, ресурса и т. п.) для управления PIM, создание списка всех управляемых ресурсов, доступных для инициатора запроса, получение отношений управляемого ресурса. | [governanceResource](governanceresource.md) | [Обнаружение ролей и управление ими](/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| Список всех ролей ресурса или получение сведений об определенной роли указанного ресурса. | [governanceRoleDefinition](governanceroledefinition.md) |  |
| Получение всех параметров роли для ресурса или обновление параметра роли. | [governanceRoleSetting](governancerolesetting.md) | [Изменение параметров роли](/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| Отображение списка и экспорт всех назначений ролей для ресурса. | [governanceRoleAssignment](governanceroleassignment.md) | [Экспорт назначений ролей](/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| Создание или удаление допустимого или активного назначения роли, активация и деактивация допустимого назначения, просмотр списка ожидающих запросов, утверждение или отказ ожидающего запроса, отмена вашего собственного ожидающего запроса. | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [Назначение ролей](/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[Активация ролей](/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[Утверждение запросов](/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

[!INCLUDE [pimv2AzureResources-migration](../../includes/pimv2AzureResources-migration.md)]

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
