---
title: тип ресурса roleManagement
description: Ресурс управления ролью RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317023"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="7a7fe-103">тип ресурса roleManagement</span><span class="sxs-lookup"><span data-stu-id="7a7fe-103">roleManagement resource type</span></span>

<span data-ttu-id="7a7fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a7fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a7fe-105">Представляет организацию Microsoft 365 ролей RBAC, которая предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у различных поставщиков RBAC.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-105">Represents a Microsoft 365 RBAC role management entity that provides access to role definitions and role assignments surfaced from various RBAC providers.</span></span> 

<span data-ttu-id="7a7fe-106">API управления единой ролью в настоящее время поддерживает следующих поставщиков RBAC в Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7a7fe-106">The unified role management API currently supports the following RBAC providers in Microsoft 365:</span></span>
- <span data-ttu-id="7a7fe-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="7a7fe-107">cloud PC</span></span> 
- <span data-ttu-id="7a7fe-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="7a7fe-108">device management (Intune)</span></span>
- <span data-ttu-id="7a7fe-109">directory (роли каталога Azure AD)</span><span class="sxs-lookup"><span data-stu-id="7a7fe-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="7a7fe-110">управление правами (управление правами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="7a7fe-110">entitlement management (Azure AD entitlement management)</span></span>
 
<span data-ttu-id="7a7fe-111">Подробнее:</span><span class="sxs-lookup"><span data-stu-id="7a7fe-111">For more information, see:</span></span> 
* [<span data-ttu-id="7a7fe-112">Роли в Microsoft 365, в том числе Azure AD, роли для служб и межуслуковые</span><span class="sxs-lookup"><span data-stu-id="7a7fe-112">Roles in Microsoft 365, including Azure AD, service-specific and cross-service roles</span></span>](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* <span data-ttu-id="7a7fe-113">[Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="7a7fe-113">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* <span data-ttu-id="7a7fe-114">[Делегирования и ролей в управлении правами Azure AD.](/azure/active-directory/governance/entitlement-management-delegate)</span><span class="sxs-lookup"><span data-stu-id="7a7fe-114">[Delegation and roles in Azure AD entitlement management](/azure/active-directory/governance/entitlement-management-delegate).</span></span>
* [<span data-ttu-id="7a7fe-115">Управление доступом на основе ролей (RBAC) в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7a7fe-115">Role-based access control (RBAC) with Microsoft Intune</span></span>](/mem/intune/fundamentals/role-based-access-control)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="7a7fe-116">Methods</span><span class="sxs-lookup"><span data-stu-id="7a7fe-116">Methods</span></span>

<span data-ttu-id="7a7fe-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-117">None.</span></span>

## <a name="properties"></a><span data-ttu-id="7a7fe-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a7fe-118">Properties</span></span>

<span data-ttu-id="7a7fe-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7a7fe-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="7a7fe-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7a7fe-120">Relationships</span></span>

| <span data-ttu-id="7a7fe-121">Связь</span><span class="sxs-lookup"><span data-stu-id="7a7fe-121">Relationship</span></span> | <span data-ttu-id="7a7fe-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7a7fe-122">Type</span></span>        | <span data-ttu-id="7a7fe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7a7fe-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a7fe-124">cloudPC</span><span class="sxs-lookup"><span data-stu-id="7a7fe-124">cloudPC</span></span>|[<span data-ttu-id="7a7fe-125">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="7a7fe-125">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)|<span data-ttu-id="7a7fe-126">Предоставляет доступ к определениям ролей и назначениям ролей поставщика облачных ПК RBAC.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-126">Provides access to role definitions and role assignments of a cloud PC RBAC provider.</span></span> <span data-ttu-id="7a7fe-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-127">Read-only.</span></span> <span data-ttu-id="7a7fe-128">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-128">Nullable.</span></span>|
|<span data-ttu-id="7a7fe-129">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7a7fe-129">deviceManagement</span></span>|[<span data-ttu-id="7a7fe-130">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="7a7fe-130">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="7a7fe-131">Предоставляет доступ к определениям ролей и назначениям ролей поставщика RBAC Intune.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-131">Provides access to role definitions and role assignments of an Intune RBAC provider.</span></span> <span data-ttu-id="7a7fe-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-132">Read-only.</span></span> <span data-ttu-id="7a7fe-133">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-133">Nullable.</span></span>|
|<span data-ttu-id="7a7fe-134">каталог</span><span class="sxs-lookup"><span data-stu-id="7a7fe-134">directory</span></span>|[<span data-ttu-id="7a7fe-135">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="7a7fe-135">rbacApplication</span></span>](rbacapplication.md)|<span data-ttu-id="7a7fe-136">Предоставляет доступ к определениям ролей и назначениям ролей поставщика Azure AD RBAC.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-136">Provides access to role definitions and role assignments of an Azure AD RBAC provider.</span></span> <span data-ttu-id="7a7fe-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-137">Read-only.</span></span> <span data-ttu-id="7a7fe-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-138">Nullable.</span></span>|
|<span data-ttu-id="7a7fe-139">entitlementManagement</span><span class="sxs-lookup"><span data-stu-id="7a7fe-139">entitlementManagement</span></span>|[<span data-ttu-id="7a7fe-140">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="7a7fe-140">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="7a7fe-141">Предоставляет доступ к определениям ролей и назначениям ролей управления правами Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-141">Provides access to role definitions and role assignments of Azure AD entitlement management.</span></span> <span data-ttu-id="7a7fe-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-142">Read-only.</span></span> <span data-ttu-id="7a7fe-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-143">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a7fe-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a7fe-144">JSON representation</span></span>

<span data-ttu-id="7a7fe-145">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a7fe-145">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
