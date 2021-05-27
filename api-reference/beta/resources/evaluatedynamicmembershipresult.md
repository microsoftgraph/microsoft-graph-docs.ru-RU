---
title: оценка типа ресурсаDynamicMembershipResult
description: Представляет результат оценки членства.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 52621ee317183a59da418ecd35309cacc0637ae3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682644"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>оценка типа ресурсаDynamicMembershipResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат оценки членства.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| membershipRule | String | Если предоставляется групповой ID, значением является правило членства для группы. Если групповой ID не предоставлен, значением является правило членства, которое было предоставлено в качестве параметра. Дополнительные сведения см. в [программе Dynamic membership rules for groups in Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership) |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Предоставляет подробный анализ результатов оценки членства. |
| membershipRuleEvaluationResult | Boolean | Значение, `true` если пользователь или устройство является членом группы. Значение также может быть, если было предоставлено правило членства и пользователь или устройство проходит оценку `true` правила; в противном случае `false` . |

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