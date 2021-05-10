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
# <a name="policyroot-resource-type"></a>тип ресурсов policyRoot

Пространство имен: microsoft.graph

Новая привязка свойств навигации для unifiedRoleManagementPolicy и unifiedRoleManagementPolicyAssignment к policyRoot.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List roleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получите ресурсы unifiedRoleManagementPolicy из свойства навигации roleManagementPolicies.|
|[List roleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)|[коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Получите ресурсы unifiedRoleManagementPolicyAssignment из свойства навигации RoleManagementPolicyAssignments.|

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

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
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

