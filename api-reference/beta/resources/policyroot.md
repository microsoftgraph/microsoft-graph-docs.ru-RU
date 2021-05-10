---
title: тип ресурсов policyRoot
description: Новая привязка свойств навигации для unifiedRoleManagementPolicy и unifiedRoleManagementPolicyAssignment к policyRoot.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85c334c52ab2bb196bcfce24610414a0843f898a
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299677"
---
# <a name="policyroot-resource-type"></a><span data-ttu-id="9e7cb-103">тип ресурсов policyRoot</span><span class="sxs-lookup"><span data-stu-id="9e7cb-103">policyRoot resource type</span></span>

<span data-ttu-id="9e7cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e7cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e7cb-105">Новая привязка свойств навигации для unifiedRoleManagementPolicy и unifiedRoleManagementPolicyAssignment к policyRoot.</span><span class="sxs-lookup"><span data-stu-id="9e7cb-105">A new navigation properties binding for unifiedRoleManagementPolicy and unifiedRoleManagementPolicyAssignment to policyRoot.</span></span>

## <a name="methods"></a><span data-ttu-id="9e7cb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9e7cb-106">Methods</span></span>
|<span data-ttu-id="9e7cb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9e7cb-107">Method</span></span>|<span data-ttu-id="9e7cb-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9e7cb-108">Return type</span></span>|<span data-ttu-id="9e7cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e7cb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e7cb-110">List roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="9e7cb-110">List roleManagementPolicies</span></span>](../api/policyroot-list-rolemanagementpolicies.md)|<span data-ttu-id="9e7cb-111">[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e7cb-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="9e7cb-112">Получите ресурсы unifiedRoleManagementPolicy из свойства навигации roleManagementPolicies.</span><span class="sxs-lookup"><span data-stu-id="9e7cb-112">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>|
|[<span data-ttu-id="9e7cb-113">List roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="9e7cb-113">List roleManagementPolicyAssignments</span></span>](../api/policyroot-list-rolemanagementpolicyassignments.md)|<span data-ttu-id="9e7cb-114">[коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e7cb-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="9e7cb-115">Получите ресурсы unifiedRoleManagementPolicyAssignment из свойства навигации RoleManagementPolicyAssignments.</span><span class="sxs-lookup"><span data-stu-id="9e7cb-115">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>|

<!--
## Properties
|Property|Type|Description|
|:---|:---|:---|


## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Represents the role management policies.|
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection|Represents the role management policy assignments.|
-->

## <a name="json-representation"></a><span data-ttu-id="9e7cb-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e7cb-116">JSON representation</span></span>
<span data-ttu-id="9e7cb-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e7cb-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

