---
title: тип ресурса unifiedRoleManagementPolicyAssignment
description: УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14c034a3cc843575d99436be7f4cb271290bf374
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695060"
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
|id|String|Уникальный идентификатор для назначения политики.|
|policyId|String|ID политики.|
|roleDefinitionId|String|ID определения роли, в котором применяется политика. Если не указано, политика применяется ко всем ролям.|
|scopeId|String|ID области, в которой назначена политика. Например, "/", groupId и т. д.|
|scopeType|String|Тип области, в которой назначена политика. Один из Directory, DirectoryRole, Group.|

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

