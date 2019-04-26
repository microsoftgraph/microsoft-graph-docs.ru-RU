---
title: Тип ресурса Рискусерактивити
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1685c58697f9de52e209d508c1ec104b9c044e8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343565"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="9dea2-102">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="9dea2-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="9dea2-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dea2-103">Properties</span></span>

| <span data-ttu-id="9dea2-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dea2-104">Property</span></span>       | <span data-ttu-id="9dea2-105">Тип</span><span class="sxs-lookup"><span data-stu-id="9dea2-105">Type</span></span>    |<span data-ttu-id="9dea2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="9dea2-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9dea2-107">Евенттипес</span><span class="sxs-lookup"><span data-stu-id="9dea2-107">eventTypes</span></span> | <span data-ttu-id="9dea2-108">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="9dea2-108">riskEventType collection</span></span> |<span data-ttu-id="9dea2-109">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="9dea2-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="9dea2-110">описаны</span><span class="sxs-lookup"><span data-stu-id="9dea2-110">detail</span></span>     | <span data-ttu-id="9dea2-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="9dea2-111">riskDetail</span></span>  | <span data-ttu-id="9dea2-112">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="9dea2-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9dea2-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dea2-113">JSON representation</span></span>

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
