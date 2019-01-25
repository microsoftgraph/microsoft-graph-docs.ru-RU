---
title: Тип ресурса риска
description: Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524823"
---
# <a name="risk-resource-type"></a>Тип ресурса риска

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
