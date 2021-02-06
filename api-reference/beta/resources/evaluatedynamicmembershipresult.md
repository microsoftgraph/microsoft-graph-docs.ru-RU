---
title: Тип ресурса evaluateDynamicMembershipResult
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1df07449605f3b1d48c01b1e352100d534fc9b1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129508"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Тип ресурса evaluateDynamicMembershipResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат оценки членства.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| membershipRule | String | Если предоставлен ИД группы, значением является правило членства для группы. Если ид группы не предоставлен, значением является правило членства, предоставленное в качестве параметра. Дополнительные сведения см. в правилах [динамического членства для групп в Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership) |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Предоставляет подробный анализ результатов оценки членства. |
| membershipRuleEvaluationResult | Boolean | Значением `true` является, если пользователь или устройство входит в группу. Значение также может быть, если предоставлено правило членства и пользователь или устройство проходят оценку правила; в противном `true` случае `false` . |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult",
  "baseType": null
}-->

```json
{
  "membershipRule": "String",
  "membershipRuleEvaluationDetails": {"@odata.type": "microsoft.graph.expressionEvaluationDetails"},
  "membershipRuleEvaluationResult": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "evaluateDynamicMembershipResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->