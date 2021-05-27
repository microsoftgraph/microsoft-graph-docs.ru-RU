---
title: тип ресурса unifiedRoleManagementPolicyAssignment
description: УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0b51d9c088a9d6da4e1a3a671dd578e07ed22691
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682623"
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

