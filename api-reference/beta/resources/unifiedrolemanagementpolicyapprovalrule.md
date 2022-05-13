---
title: Тип ресурса unifiedRoleManagementPolicyApprovalRule
description: UnifiedRoleManagementPolicyApprovalRule указывает правило утверждения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a48917590c966424473258b9d40af432f98bf917
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397560"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyApprovalRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyApprovalRule указывает правило утверждения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|setting|[approvalSettings](../resources/approvalsettings.md)|Параметр утверждения для правила.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

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

