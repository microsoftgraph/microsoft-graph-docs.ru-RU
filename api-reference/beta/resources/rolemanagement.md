---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 19eb561944c3d9055f8453906bfedb92701c814f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016170"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="e88db-103">Тип ресурса Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="e88db-103">roleManagement resource type</span></span>

<span data-ttu-id="e88db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e88db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e88db-105">Представляет объект управления ролями Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="e88db-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="e88db-106">Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC.</span><span class="sxs-lookup"><span data-stu-id="e88db-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="e88db-107">В настоящее время поддерживаются поставщики Active Directory (Azure AD) и deviceManagement (Intune).</span><span class="sxs-lookup"><span data-stu-id="e88db-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="e88db-108">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="e88db-108">For more information, see:</span></span> 
* <span data-ttu-id="e88db-109">[Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="e88db-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="e88db-110">Управление доступом на основе ролей (RBAC) в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e88db-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="e88db-111">Методы</span><span class="sxs-lookup"><span data-stu-id="e88db-111">Methods</span></span>

<span data-ttu-id="e88db-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="e88db-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="e88db-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e88db-113">Properties</span></span>

<span data-ttu-id="e88db-114">Нет</span><span class="sxs-lookup"><span data-stu-id="e88db-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e88db-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e88db-115">Relationships</span></span>

| <span data-ttu-id="e88db-116">Связь</span><span class="sxs-lookup"><span data-stu-id="e88db-116">Relationship</span></span> | <span data-ttu-id="e88db-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e88db-117">Type</span></span>        | <span data-ttu-id="e88db-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e88db-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e88db-119">каталога</span><span class="sxs-lookup"><span data-stu-id="e88db-119">directory</span></span>|[<span data-ttu-id="e88db-120">рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="e88db-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="e88db-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88db-121">Read-only.</span></span> <span data-ttu-id="e88db-122">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e88db-122">Nullable.</span></span>|
|<span data-ttu-id="e88db-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e88db-123">deviceManagement</span></span>|[<span data-ttu-id="e88db-124">рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="e88db-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="e88db-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e88db-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e88db-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e88db-127">JSON representation</span></span>

<span data-ttu-id="e88db-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="e88db-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


