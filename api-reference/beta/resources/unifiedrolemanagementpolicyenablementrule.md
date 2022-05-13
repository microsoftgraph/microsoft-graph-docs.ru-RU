---
title: Тип ресурса unifiedRoleManagementPolicyEnablementRule
description: UnifiedRoleManagementPolicyEnablementRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5a709aedb9d0a6b819fffe2edf4ce5a217f20ba4
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397742"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyEnablementRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyEnablementRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enabledRules|Коллекция String|Включенные правила. Допустимые значения: MultifactorAuthentication, Justification, Ticketing.|
|id|String|Уникальный идентификатор правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

