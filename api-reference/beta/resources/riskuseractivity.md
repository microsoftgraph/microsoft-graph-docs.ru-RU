---
title: Тип ресурса Рискусерактивити
description: author
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1601f34b7d54a2c5304f3b20b04b8cb4c69c6323
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521070"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="c2693-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="c2693-103">riskUserActivity resource type</span></span>

<span data-ttu-id="c2693-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2693-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="c2693-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2693-105">Properties</span></span>

| <span data-ttu-id="c2693-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2693-106">Property</span></span>       | <span data-ttu-id="c2693-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c2693-107">Type</span></span>    |<span data-ttu-id="c2693-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c2693-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2693-109">евенттипес</span><span class="sxs-lookup"><span data-stu-id="c2693-109">eventTypes</span></span> | <span data-ttu-id="c2693-110">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="c2693-110">riskEventType collection</span></span> |<span data-ttu-id="c2693-111">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="c2693-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="c2693-112">описаны</span><span class="sxs-lookup"><span data-stu-id="c2693-112">detail</span></span>     | <span data-ttu-id="c2693-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c2693-113">riskDetail</span></span>  | <span data-ttu-id="c2693-114">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="c2693-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c2693-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2693-115">JSON representation</span></span>

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
