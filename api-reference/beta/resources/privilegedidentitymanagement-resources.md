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
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="62be3-103">Privileged Identity Management — ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="62be3-103">Privileged Identity Management - Azure resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62be3-104">Можно использовать службу [Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) для ресурсов Azure, чтобы настроить рабочий процесс своевременного предоставления доступа для ролей инфраструктуры Azure на уровне групп управления, подписок, групп ресурсов и отдельных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="62be3-104">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="62be3-105">Это относится как ко встроенным ролям, таким как "Владелец" и "Участник", так и к настраиваемым ролям RBAC.</span><span class="sxs-lookup"><span data-stu-id="62be3-105">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="62be3-106">Основные варианты использования службы PIM и ресурсов Azure с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="62be3-106">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="62be3-107">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="62be3-107">Use case</span></span> | <span data-ttu-id="62be3-108">Ресурс</span><span class="sxs-lookup"><span data-stu-id="62be3-108">Resource</span></span> | <span data-ttu-id="62be3-109">См. также</span><span class="sxs-lookup"><span data-stu-id="62be3-109">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="62be3-110">Подключение ресурса (подписок, группы ресурсов, ресурса и т. п.) для управления PIM, создание списка всех управляемых ресурсов, доступных для инициатора запроса, получение отношений управляемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="62be3-110">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="62be3-111">governanceResource</span><span class="sxs-lookup"><span data-stu-id="62be3-111">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="62be3-112">Обнаружение ролей и управление ими</span><span class="sxs-lookup"><span data-stu-id="62be3-112">Role discovery and management</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="62be3-113">Список всех ролей ресурса или получение сведений об определенной роли указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="62be3-113">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="62be3-114">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="62be3-114">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="62be3-115">Получение всех параметров роли для ресурса или обновление параметра роли.</span><span class="sxs-lookup"><span data-stu-id="62be3-115">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="62be3-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="62be3-116">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="62be3-117">Изменение параметров роли</span><span class="sxs-lookup"><span data-stu-id="62be3-117">Configure role setting</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="62be3-118">Отображение списка и экспорт всех назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="62be3-118">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="62be3-119">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="62be3-119">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="62be3-120">Экспорт назначений ролей</span><span class="sxs-lookup"><span data-stu-id="62be3-120">Export role assignments</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="62be3-121">Создание или удаление допустимого или активного назначения роли, активация и деактивация допустимого назначения, просмотр списка ожидающих запросов, утверждение или отказ ожидающего запроса, отмена вашего собственного ожидающего запроса.</span><span class="sxs-lookup"><span data-stu-id="62be3-121">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="62be3-122">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="62be3-122">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="62be3-123">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="62be3-123">Role assignment</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="62be3-124">Активация ролей</span><span class="sxs-lookup"><span data-stu-id="62be3-124">Role activation</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="62be3-125">Утверждение запросов</span><span class="sxs-lookup"><span data-stu-id="62be3-125">Approve or deny requests</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
