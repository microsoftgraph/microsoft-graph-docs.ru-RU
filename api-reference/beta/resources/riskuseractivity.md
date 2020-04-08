---
title: Тип ресурса Рискусерактивити
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26dc0cf4d8309e2cc116b4b4265a3d592d316a56
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178910"
---
# <a name="riskuseractivity-resource-type"></a>Тип ресурса Рискусерактивити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| евенттипес | Коллекция Рискевенттипе |Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.  |
| описаны     | riskDetail  | Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.  |

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
