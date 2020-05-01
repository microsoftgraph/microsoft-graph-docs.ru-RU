---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 71c59c1e44123b60dd46b2c72e71aabfc7a64c25
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991784"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="9dc8e-103">Тип ресурса Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="9dc8e-103">roleManagement resource type</span></span>

<span data-ttu-id="9dc8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dc8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc8e-105">Представляет объект управления ролями Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="9dc8e-106">Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="9dc8e-107">В настоящее время поддерживаются поставщики Active Directory (Azure AD) и deviceManagement (Intune).</span><span class="sxs-lookup"><span data-stu-id="9dc8e-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="9dc8e-108">Дополнительные сведения см. в статье:</span><span class="sxs-lookup"><span data-stu-id="9dc8e-108">For more information, see:</span></span> 
* <span data-ttu-id="9dc8e-109">[Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="9dc8e-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="9dc8e-110">Управление доступом на основе ролей (RBAC) в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9dc8e-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="9dc8e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9dc8e-111">Methods</span></span>

<span data-ttu-id="9dc8e-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="9dc8e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dc8e-113">Properties</span></span>

<span data-ttu-id="9dc8e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="9dc8e-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="9dc8e-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="9dc8e-115">Relationships</span></span>

| <span data-ttu-id="9dc8e-116">Связь</span><span class="sxs-lookup"><span data-stu-id="9dc8e-116">Relationship</span></span> | <span data-ttu-id="9dc8e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc8e-117">Type</span></span>        | <span data-ttu-id="9dc8e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc8e-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9dc8e-119">каталога</span><span class="sxs-lookup"><span data-stu-id="9dc8e-119">directory</span></span>|[<span data-ttu-id="9dc8e-120">рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="9dc8e-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="9dc8e-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-121">Read-only.</span></span> <span data-ttu-id="9dc8e-122">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-122">Nullable.</span></span>|
|<span data-ttu-id="9dc8e-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9dc8e-123">deviceManagement</span></span>|[<span data-ttu-id="9dc8e-124">рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="9dc8e-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="9dc8e-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dc8e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dc8e-127">JSON representation</span></span>

<span data-ttu-id="9dc8e-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="9dc8e-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
