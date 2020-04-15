---
title: Тип ресурса Рискусерактивити
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ddf71668af9d66c1d3ea495a8438c444b9317a23
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510996"
---
# <a name="riskuseractivity-resource-type"></a>Тип ресурса Рискусерактивити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| евенттипес | Коллекция Рискевенттипе |Список типов событий риска. Устаревшие. Вместо этого используйте **рискевенттипес** . |
|рискевенттипе|string|Тип обнаруженного события риска. Возможные значения: `unlikelyTravel` `anonymizedIPAddress`,, `maliciousIPAddress`, `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials`,,,, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `unknownFutureValue`,,,, и. `maliciousIPAddressValidCredentialsBlockedIP` |
| описаны     | riskDetail  | Возможные значения: `none` `adminGeneratedTemporaryPassword`,, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminConfirmedUserCompromised` `unknownFutureValue`,,,,,,,,. `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden`  |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
    "detail": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->
