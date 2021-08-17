---
title: тип ресурса unifiedRoleManagementPolicyAssignment
description: УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1d35d2937e0636803a82d5b47bc2db165b677baf04936de46d11bc4ff87b00f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145133"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>тип ресурса unifiedRoleManagementPolicyAssignment

УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleManagementPolicyAssignments](../api/unifiedrolemanagementpolicyassignment-list.md)|[коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Получите список объектов [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) и их свойств.|
|[Get unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Ознакомьтесь с свойствами и отношениями единого [объектаRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для назначения политики.|
|policyId|String|ID политики.|
|roleDefinitionId|Строка|ID определения роли, в котором применяется политика. Если не указано, политика применяется ко всем ролям.|
|scopeId|Строка|ID области, в которой назначена политика. Например, "/", groupId и т. д.|
|scopeType|Строка|Тип области, в которой назначена политика. Один из Directory, DirectoryRole, Group.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policy|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Политика назначения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

