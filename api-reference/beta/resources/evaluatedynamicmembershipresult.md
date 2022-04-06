---
title: оценка типа ресурсаDynamicMembershipResult
description: Представляет результат оценки членства.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 551c2c87a09b7f2ddafc2079ab97c7f7e36837cd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588528"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>оценка типа ресурсаDynamicMembershipResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат оценки членства.

## <a name="properties"></a>Свойства

| Свойство                        | Тип                                                          | Описание                                                                                                                                                                                                                                                                                                                                   |
| :------------------------------ | :------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| membershipRule                  | String                                                        | Если предоставляется групповой ID, значением является правило членства для группы. Если групповой ID не предоставлен, значением является правило членства, которое было предоставлено в качестве параметра. Дополнительные сведения можно найти в статье [Правила динамического членства в группах для Azure AD](/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Предоставляет подробный анализ результатов оценки членства.                                                                                                                                                                                                                                                                             |
| membershipRuleEvaluationResult  | Логический                                                       | Значение, если `true` пользователь или устройство является членом группы. Значение также может быть, `true` если было предоставлено правило членства и пользователь или устройство проходит оценку правила; в противном случае `false`.                                                                                                                                      |

## <a name="json-representation"></a>Представление JSON

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
  "membershipRuleEvaluationDetails": {
    "@odata.type": "microsoft.graph.expressionEvaluationDetails"
  },
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
