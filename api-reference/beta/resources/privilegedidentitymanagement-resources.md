---
title: Privileged Identity Management — ресурсы Azure
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ресурсами Azure.
localization_priority: Priority
author: shauliu
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 83ffad748b6a7b08fbdd8a4578369410c219d453
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219216"
---
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="10e2b-103">Privileged Identity Management — ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="10e2b-103">Privileged Identity Management - Azure resources</span></span>

<span data-ttu-id="10e2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10e2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e2b-105">Можно использовать службу [Privileged Identity Management (PIM) Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) для ресурсов Azure, чтобы настроить рабочий процесс своевременного предоставления доступа для ролей инфраструктуры Azure на уровне групп управления, подписок, групп ресурсов и отдельных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="10e2b-105">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="10e2b-106">Это относится как ко встроенным ролям, таким как "Владелец" и "Участник", так и к настраиваемым ролям RBAC.</span><span class="sxs-lookup"><span data-stu-id="10e2b-106">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="10e2b-107">Основные варианты использования службы PIM и ресурсов Azure с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="10e2b-107">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="10e2b-108">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="10e2b-108">Use case</span></span> | <span data-ttu-id="10e2b-109">Ресурс</span><span class="sxs-lookup"><span data-stu-id="10e2b-109">Resource</span></span> | <span data-ttu-id="10e2b-110">См. также</span><span class="sxs-lookup"><span data-stu-id="10e2b-110">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="10e2b-111">Подключение ресурса (подписок, группы ресурсов, ресурса и т. п.) для управления PIM, создание списка всех управляемых ресурсов, доступных для инициатора запроса, получение отношений управляемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="10e2b-111">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="10e2b-112">governanceResource</span><span class="sxs-lookup"><span data-stu-id="10e2b-112">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="10e2b-113">Обнаружение ролей и управление ими</span><span class="sxs-lookup"><span data-stu-id="10e2b-113">Role discovery and management</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="10e2b-114">Список всех ролей ресурса или получение сведений об определенной роли указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="10e2b-114">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="10e2b-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10e2b-115">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="10e2b-116">Получение всех параметров роли для ресурса или обновление параметра роли.</span><span class="sxs-lookup"><span data-stu-id="10e2b-116">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="10e2b-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="10e2b-117">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="10e2b-118">Изменение параметров роли</span><span class="sxs-lookup"><span data-stu-id="10e2b-118">Configure role setting</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="10e2b-119">Отображение списка и экспорт всех назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="10e2b-119">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="10e2b-120">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="10e2b-120">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="10e2b-121">Экспорт назначений ролей</span><span class="sxs-lookup"><span data-stu-id="10e2b-121">Export role assignments</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="10e2b-122">Создание или удаление допустимого или активного назначения роли, активация и деактивация допустимого назначения, просмотр списка ожидающих запросов, утверждение или отказ ожидающего запроса, отмена вашего собственного ожидающего запроса.</span><span class="sxs-lookup"><span data-stu-id="10e2b-122">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="10e2b-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="10e2b-123">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="10e2b-124">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="10e2b-124">Role Assignment</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="10e2b-125">Активация ролей</span><span class="sxs-lookup"><span data-stu-id="10e2b-125">Role activation</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="10e2b-126">Утверждение запросов</span><span class="sxs-lookup"><span data-stu-id="10e2b-126">Approve requests</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
