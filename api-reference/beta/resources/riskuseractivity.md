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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="5871e-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="5871e-103">riskUserActivity resource type</span></span>

<span data-ttu-id="5871e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5871e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="5871e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5871e-105">Properties</span></span>

| <span data-ttu-id="5871e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5871e-106">Property</span></span>       | <span data-ttu-id="5871e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5871e-107">Type</span></span>    |<span data-ttu-id="5871e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5871e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5871e-109">евенттипес</span><span class="sxs-lookup"><span data-stu-id="5871e-109">eventTypes</span></span> | <span data-ttu-id="5871e-110">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="5871e-110">riskEventType collection</span></span> |<span data-ttu-id="5871e-111">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="5871e-111">List of risk event types.</span></span> <span data-ttu-id="5871e-112">Устаревшие.</span><span class="sxs-lookup"><span data-stu-id="5871e-112">Deprecated.</span></span> <span data-ttu-id="5871e-113">Вместо этого используйте **рискевенттипес** .</span><span class="sxs-lookup"><span data-stu-id="5871e-113">Use **riskEventTypes** instead.</span></span> |
|<span data-ttu-id="5871e-114">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="5871e-114">riskEventType</span></span>|<span data-ttu-id="5871e-115">string</span><span class="sxs-lookup"><span data-stu-id="5871e-115">string</span></span>|<span data-ttu-id="5871e-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="5871e-116">The type of risk event detected.</span></span> <span data-ttu-id="5871e-117">Возможные значения: `unlikelyTravel` `anonymizedIPAddress`,, `maliciousIPAddress`, `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials`,,,, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `unknownFutureValue`,,,, и. `maliciousIPAddressValidCredentialsBlockedIP`</span><span class="sxs-lookup"><span data-stu-id="5871e-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="5871e-118">описаны</span><span class="sxs-lookup"><span data-stu-id="5871e-118">detail</span></span>     | <span data-ttu-id="5871e-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5871e-119">riskDetail</span></span>  | <span data-ttu-id="5871e-120">Возможные значения: `none` `adminGeneratedTemporaryPassword`,, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminConfirmedUserCompromised` `unknownFutureValue`,,,,,,,,. `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden`</span><span class="sxs-lookup"><span data-stu-id="5871e-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5871e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5871e-121">JSON representation</span></span>

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
