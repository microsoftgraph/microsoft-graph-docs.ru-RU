---
title: Тип ресурса unifiedRoleManagementPolicyAssignment
description: UnifiedRoleManagementPolicyAssignment назначает политику определенной области и определению роли.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8dfbe842f6e60abec9c0f15881695062e901d5ba
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446317"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAssignment

Пространство имен: microsoft.graph

Назначение политики управления ролем [объекту определения](../resources/unifiedroledefinition.md) роли.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleManagementPolicyAssignment](../api/policyroot-list-rolemanagementpolicyassignments.md)|[Коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Получение сведений о всех назначениях политик управления ролами, включая политики и правила, связанные с Azure AD роли.|
|[Получение объекта unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Чтение свойств и связей объекта [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор назначения политики. Идентификатор обычно представляет собой объединение идентификатора unifiedRoleManagementPolicy и roleDefinitionId, разделенных символом подчеркивания.|
|policyId|String|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|roleDefinitionId|String|Идентификатор объекта [определения роли,](unifiedroledefinition.md) к которому применяется политика. Если этот параметр не указан, политика применяется ко всем ролям. Поддерживает $filter (`eq`).|
|scopeId|String|Идентификатор области, в которой назначена политика.  Может быть `/` для клиента или идентификатора группы. Обязательный элемент.|
|scopeType|String|Тип области, в которой назначена политика. Один из `Directory`, `DirectoryRole`. Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policy|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Политика, связанная с назначением политики. Поддерживает $expand и вложенную $expand правил и связей effectiveRules для политики.|

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

