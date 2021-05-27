---
title: тип ресурсов policyRoot
description: Новая привязка свойств навигации для unifiedRoleManagementPolicy и unifiedRoleManagementPolicyAssignment к policyRoot.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3827440befd26fb584addd0d6af520a6498c11dd
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680727"
---
# <a name="policyroot-resource-type"></a><span data-ttu-id="1d068-103">тип ресурсов policyRoot</span><span class="sxs-lookup"><span data-stu-id="1d068-103">policyRoot resource type</span></span>

<span data-ttu-id="1d068-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d068-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d068-105">Новая привязка свойств навигации для unifiedRoleManagementPolicy и unifiedRoleManagementPolicyAssignment к policyRoot.</span><span class="sxs-lookup"><span data-stu-id="1d068-105">A new navigation properties binding for unifiedRoleManagementPolicy and unifiedRoleManagementPolicyAssignment to policyRoot.</span></span>

## <a name="methods"></a><span data-ttu-id="1d068-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1d068-106">Methods</span></span>
|<span data-ttu-id="1d068-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1d068-107">Method</span></span>|<span data-ttu-id="1d068-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="1d068-108">Return type</span></span>|<span data-ttu-id="1d068-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1d068-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d068-110">List roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="1d068-110">List roleManagementPolicies</span></span>](../api/policyroot-list-rolemanagementpolicies.md)|<span data-ttu-id="1d068-111">[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d068-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="1d068-112">Получите ресурсы unifiedRoleManagementPolicy из свойства навигации roleManagementPolicies.</span><span class="sxs-lookup"><span data-stu-id="1d068-112">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>|
|[<span data-ttu-id="1d068-113">List roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="1d068-113">List roleManagementPolicyAssignments</span></span>](../api/policyroot-list-rolemanagementpolicyassignments.md)|<span data-ttu-id="1d068-114">[коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d068-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="1d068-115">Получите ресурсы unifiedRoleManagementPolicyAssignment из свойства навигации RoleManagementPolicyAssignments.</span><span class="sxs-lookup"><span data-stu-id="1d068-115">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>|

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

## <a name="json-representation"></a><span data-ttu-id="1d068-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d068-116">JSON representation</span></span>
<span data-ttu-id="1d068-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d068-117">The following is a JSON representation of the resource.</span></span>
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

