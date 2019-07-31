---
title: Тип ресурса Рискусерактивити
description: author
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4b33d4f9344f8031076f00b1b442b882fffe6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965357"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="5a7cc-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="5a7cc-103">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="5a7cc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a7cc-104">Properties</span></span>

| <span data-ttu-id="5a7cc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a7cc-105">Property</span></span>       | <span data-ttu-id="5a7cc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5a7cc-106">Type</span></span>    |<span data-ttu-id="5a7cc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="5a7cc-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a7cc-108">Евенттипес</span><span class="sxs-lookup"><span data-stu-id="5a7cc-108">eventTypes</span></span> | <span data-ttu-id="5a7cc-109">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="5a7cc-109">riskEventType collection</span></span> |<span data-ttu-id="5a7cc-110">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, Generic Админконфирмедусеркомпромисед, Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="5a7cc-110">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="5a7cc-111">описаны</span><span class="sxs-lookup"><span data-stu-id="5a7cc-111">detail</span></span>     | <span data-ttu-id="5a7cc-112">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5a7cc-112">riskDetail</span></span>  | <span data-ttu-id="5a7cc-113">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="5a7cc-113">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5a7cc-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a7cc-114">JSON representation</span></span>

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
