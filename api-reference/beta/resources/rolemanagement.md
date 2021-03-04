---
title: тип ресурса roleManagement
description: Ресурс управления ролью RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440131"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="0774c-103">тип ресурса roleManagement</span><span class="sxs-lookup"><span data-stu-id="0774c-103">roleManagement resource type</span></span>

<span data-ttu-id="0774c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0774c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0774c-105">Представляет сущность управления ролью Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="0774c-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="0774c-106">Предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у поставщиков RBAC.</span><span class="sxs-lookup"><span data-stu-id="0774c-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="0774c-107">В настоящее время поддерживаются поставщики каталогов (Azure AD) и deviceManagement (Intune).</span><span class="sxs-lookup"><span data-stu-id="0774c-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="0774c-108">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="0774c-108">For more information, see:</span></span> 
* <span data-ttu-id="0774c-109">[Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="0774c-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="0774c-110">Управление доступом на основе ролей (RBAC) с Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0774c-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="0774c-111">Methods</span><span class="sxs-lookup"><span data-stu-id="0774c-111">Methods</span></span>

<span data-ttu-id="0774c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="0774c-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="0774c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="0774c-113">Properties</span></span>

<span data-ttu-id="0774c-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0774c-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0774c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="0774c-115">Relationships</span></span>

| <span data-ttu-id="0774c-116">Связь</span><span class="sxs-lookup"><span data-stu-id="0774c-116">Relationship</span></span> | <span data-ttu-id="0774c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0774c-117">Type</span></span>        | <span data-ttu-id="0774c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0774c-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0774c-119">каталог</span><span class="sxs-lookup"><span data-stu-id="0774c-119">directory</span></span>|[<span data-ttu-id="0774c-120">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="0774c-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="0774c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0774c-121">Read-only.</span></span> <span data-ttu-id="0774c-122">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0774c-122">Nullable.</span></span>|
|<span data-ttu-id="0774c-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0774c-123">deviceManagement</span></span>|[<span data-ttu-id="0774c-124">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="0774c-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="0774c-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0774c-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0774c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0774c-127">JSON representation</span></span>

<span data-ttu-id="0774c-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="0774c-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
