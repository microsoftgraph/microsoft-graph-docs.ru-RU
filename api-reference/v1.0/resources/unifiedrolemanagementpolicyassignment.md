---
title: Тип ресурса unifiedRoleManagementPolicyAssignment
description: Назначение политики управления ролем объекту определения роли.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 813e0bd3ec6c5327f3bd0028d9b1c8c59eab5c5d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134469"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAssignment

Пространство имен: microsoft.graph

Назначение политики управления ролем [объекту определения](../resources/unifiedroledefinition.md) роли.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleManagementPolicyAssignment](../api/policyroot-list-rolemanagementpolicyassignments.md)|[Коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Получение списка объектов [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) и их свойств.|
|[Получение объекта unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Чтение свойств и связей объекта [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) .|

<!--
|[Create unifiedRoleManagementPolicyAssignment](../api/policyroot-post-rolemanagementpolicyassignments.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Create a new [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[Update unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-update.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Update the properties of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[Delete unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-delete.md)|None|Deletes an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[List unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicyassignment-list-policy.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Get the unifiedRoleManagementPolicy resources from the policy navigation property.|
|[Add unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicyassignment-post-policy.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Add policy by posting to the policy collection.|
-->

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор назначения политики. Идентификатор обычно представляет собой объединение идентификатора **unifiedRoleManagementPolicy** и **roleDefinitionId** , разделенных символом подчеркивания.|
|policyId|String|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|roleDefinitionId|String|Идентификатор объекта [определения роли,](unifiedroledefinition.md) к которому применяется политика. Если этот параметр не указан, политика применяется ко всем ролям. Поддерживает $filter (`eq`).|
|scopeId|String|Идентификатор области, в которой назначена политика.  Может быть `/` для клиента или идентификатора группы. Обязательный.|
|scopeType|String|Тип области, в которой назначена политика. Один из `Directory`, `DirectoryRole`. Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policy|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)| Политика, связанная с назначением политики. Поддерживает и `$expand` вложенные `$expand` правила **и** **эффективные отношенияrules** для политики.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "baseType": "microsoft.graph.entity",
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

