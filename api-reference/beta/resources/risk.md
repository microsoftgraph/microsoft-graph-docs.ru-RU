---
title: Тип ресурса риска
description: Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.
ms.openlocfilehash: bc8ea5c30f78560ae8750e7750596f282feb4825
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077416"
---
# <a name="risk-resource-type"></a>Тип ресурса риска

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Description|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент. |
|`riskLevelAggregated`|riskLevel|Предоставляет общий уровень риска рискованный пользователя, входа или события риска. Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`. Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.|
|`riskLevelDuringSignIn`|riskLeve|Обеспечивает уровень риска входа в при входе в систему (то есть на основании события рисков в режиме реального времени). Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`. Значение `hidden` означает, что входа в не был включен для защиты удостоверения Azure AD.|
|`state`|riskState|Предоставляет «состояние риска» рискованный пользователя, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
