---
title: Тип ресурса Евалуатединамикмембершипресулт
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a38ae33d59ea8deba8a71e48698baeddf709ae9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071238"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Тип ресурса Евалуатединамикмембершипресулт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат оценки членства.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| membershipRule | String | Если указан идентификатор группы, то значение является правилом членства для группы. Если идентификатор группы не указан, то значением является правило членства, предоставленное в качестве параметра. Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| мембершипруливалуатиондетаилс | [expressionEvaluationDetails](expressionevaluationdetails.md) | Предоставляет подробные анайлсис результатов оценки членства. |
| мембершипруливалуатионресулт | Boolean | Значение, `true` Если пользователь или устройство является участником группы. Значение также может быть `true` указано в том случае, если было предоставлено правило членства, и пользователь или устройство проходят оценку правила; в противном случае — значение `false` . |

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

