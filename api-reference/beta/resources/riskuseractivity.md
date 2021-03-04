---
title: тип ресурса riskUserActivity
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7772bde328004ffd26133421cc97a9f296ae9370
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442875"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="e6860-103">тип ресурса riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="e6860-103">riskUserActivity resource type</span></span>

<span data-ttu-id="e6860-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6860-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="e6860-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6860-105">Properties</span></span>

| <span data-ttu-id="e6860-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6860-106">Property</span></span>       | <span data-ttu-id="e6860-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e6860-107">Type</span></span>    |<span data-ttu-id="e6860-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e6860-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6860-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="e6860-109">eventTypes</span></span> | <span data-ttu-id="e6860-110">коллекция riskEventType</span><span class="sxs-lookup"><span data-stu-id="e6860-110">riskEventType collection</span></span> |<span data-ttu-id="e6860-111">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="e6860-111">List of risk event types.</span></span> <span data-ttu-id="e6860-112">Устарело.</span><span class="sxs-lookup"><span data-stu-id="e6860-112">Deprecated.</span></span> <span data-ttu-id="e6860-113">Вместо **этого используйте riskEventType.**</span><span class="sxs-lookup"><span data-stu-id="e6860-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="e6860-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e6860-114">riskEventType</span></span>|<span data-ttu-id="e6860-115">string</span><span class="sxs-lookup"><span data-stu-id="e6860-115">string</span></span>|<span data-ttu-id="e6860-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="e6860-116">The type of risk event detected.</span></span> <span data-ttu-id="e6860-117">Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="e6860-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="e6860-118">подробные</span><span class="sxs-lookup"><span data-stu-id="e6860-118">detail</span></span>     | <span data-ttu-id="e6860-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e6860-119">riskDetail</span></span>  | <span data-ttu-id="e6860-120">Возможные `none` значения: `adminGeneratedTemporaryPassword` , `userPerformedSecuredPasswordChange` , , , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` , `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` , .</span><span class="sxs-lookup"><span data-stu-id="e6860-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e6860-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6860-121">JSON representation</span></span>

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


