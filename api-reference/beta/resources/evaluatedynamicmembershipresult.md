---
title: Тип ресурса Евалуатединамикмембершипресулт
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6e40c796468a8c31d2cd75dd2b6815440bfb71e
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272853"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Тип ресурса Евалуатединамикмембершипресулт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат оценки членства.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| membershipRule | String | Если указан идентификатор группы, то значение является правилом членства для группы. Если идентификатор группы не указан, то значением является правило членства, предоставленное в качестве параметра. Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| мембершипруливалуатиондетаилс | [експрессионевалуатиондетаилс](expressionevaluationdetails.md) | Предоставляет подробные анайлсис результатов оценки членства. |
| мембершипруливалуатионресулт | Логический | Значение, `true` Если пользователь или устройство является участником группы. Значение также может быть `true` указано в том случае, если было предоставлено правило членства, и пользователь или устройство проходят оценку правила; в противном случае — значение `false` . |

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