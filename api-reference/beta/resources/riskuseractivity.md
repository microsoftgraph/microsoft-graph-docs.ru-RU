---
title: Тип ресурса Рискусерактивити
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563020"
---
# <a name="riskuseractivity-resource-type"></a>Тип ресурса Рискусерактивити

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| Евенттипес | Коллекция Рискевенттипе |Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.  |
| описаны     | riskDetail  | Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.  |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": [{"@odata.type":"microsoft.graph.riskEventType"}],
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
