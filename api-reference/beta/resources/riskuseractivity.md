---
title: Тип ресурса Рискусерактивити
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31688512"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="d277f-102">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="d277f-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="d277f-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="d277f-103">Properties</span></span>

| <span data-ttu-id="d277f-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="d277f-104">Property</span></span>       | <span data-ttu-id="d277f-105">Тип</span><span class="sxs-lookup"><span data-stu-id="d277f-105">Type</span></span>    |<span data-ttu-id="d277f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="d277f-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d277f-107">Евенттипес</span><span class="sxs-lookup"><span data-stu-id="d277f-107">eventTypes</span></span> | <span data-ttu-id="d277f-108">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="d277f-108">riskEventType collection</span></span> |<span data-ttu-id="d277f-109">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="d277f-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="d277f-110">описаны</span><span class="sxs-lookup"><span data-stu-id="d277f-110">detail</span></span>     | <span data-ttu-id="d277f-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="d277f-111">riskDetail</span></span>  | <span data-ttu-id="d277f-112">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="d277f-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d277f-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d277f-113">JSON representation</span></span>

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
