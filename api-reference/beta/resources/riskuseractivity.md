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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="550fb-102">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="550fb-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="550fb-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="550fb-103">Properties</span></span>

| <span data-ttu-id="550fb-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="550fb-104">Property</span></span>       | <span data-ttu-id="550fb-105">Тип</span><span class="sxs-lookup"><span data-stu-id="550fb-105">Type</span></span>    |<span data-ttu-id="550fb-106">Описание</span><span class="sxs-lookup"><span data-stu-id="550fb-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="550fb-107">Евенттипес</span><span class="sxs-lookup"><span data-stu-id="550fb-107">eventTypes</span></span> | <span data-ttu-id="550fb-108">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="550fb-108">riskEventType collection</span></span> |<span data-ttu-id="550fb-109">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="550fb-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="550fb-110">описаны</span><span class="sxs-lookup"><span data-stu-id="550fb-110">detail</span></span>     | <span data-ttu-id="550fb-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="550fb-111">riskDetail</span></span>  | <span data-ttu-id="550fb-112">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="550fb-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="550fb-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="550fb-113">JSON representation</span></span>

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
