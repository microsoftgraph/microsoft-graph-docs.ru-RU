---
title: Тип ресурса unifiedRoleManagementPolicyAssignment
description: UnifiedRoleManagementPolicyAssignment назначает политику определенной области и определению роли.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 93dffd5526332af16f8516e0e5a1b81a773e47d9
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397294"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAssignment

UnifiedRoleManagementPolicyAssignment назначает политику определенной области и определению роли.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-list.md)|[Коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Получение списка объектов [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) и их свойств.|
|[Получение объекта unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Чтение свойств и связей объекта [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор назначения политики.|
|policyId|String|Идентификатор политики.|
|roleDefinitionId|String|Идентификатор определения роли, к которому применяется политика. Если этот параметр не указан, политика применяется ко всем ролям.|
|scopeId|String|Идентификатор области, в которой назначена политика. Например, "/", groupId и т. д.|
|scopeType|String|Тип области, в которой назначена политика. Один из каталогов, DirectoryRole, Group.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policy|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Политика для назначения.|

## <a name="json-representation"></a>Представление в формате JSON
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

