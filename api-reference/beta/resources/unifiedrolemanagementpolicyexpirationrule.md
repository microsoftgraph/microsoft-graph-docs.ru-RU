---
title: Тип ресурса unifiedRoleManagementPolicyExpirationRule
description: UnifiedRoleManagementPolicyExpirationRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0863441c71fea62f4d5f48980f5d1494f2d0a001
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397301"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyExpirationRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyExpirationRule указывает правило включения, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|isExpirationRequired|Логический|Указывает, требуется ли истечение срока действия для соответствия требованиям или назначения.|
|maximumDuration|Длительность|Максимальная длительность, допустимая для соответствия требованиям или назначения, которая не является постоянной.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

