---
title: Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: UnifiedRoleManagementPolicyAuthenticationContextRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5e99ef993d846162cdd25a6207474629733865d4
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398842"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyAuthenticationContextRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|claimValue|String|Значение утверждения контекста проверки подлинности.|
|id|String|Уникальный идентификатор правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|isEnabled|Boolean|Указывает, включен ли параметр.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

