---
title: тип ресурса unifiedRoleManagementPolicyApprovalRule
description: Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f2777045f45c38274f5a1efa750ea276e744b781
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510171"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a>тип ресурса unifiedRoleManagementPolicyApprovalRule

Пространство имен: microsoft.graph

Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.

Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|setting|[approvalSettings](../resources/approvalsettings.md)|Параметр утверждения правила.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Цель правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

