---
title: Тип ресурса Рискусерактивити
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8032a721a8f8a94d7cd1481edf58ee785092bcfd
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556319"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="0ef5e-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="0ef5e-103">riskUserActivity resource type</span></span>

<span data-ttu-id="0ef5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ef5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="0ef5e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ef5e-105">Properties</span></span>

| <span data-ttu-id="0ef5e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ef5e-106">Property</span></span>       | <span data-ttu-id="0ef5e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0ef5e-107">Type</span></span>    |<span data-ttu-id="0ef5e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0ef5e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ef5e-109">евенттипес</span><span class="sxs-lookup"><span data-stu-id="0ef5e-109">eventTypes</span></span> | <span data-ttu-id="0ef5e-110">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="0ef5e-110">riskEventType collection</span></span> |<span data-ttu-id="0ef5e-111">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="0ef5e-111">List of risk event types.</span></span> <span data-ttu-id="0ef5e-112">Устаревшие.</span><span class="sxs-lookup"><span data-stu-id="0ef5e-112">Deprecated.</span></span> <span data-ttu-id="0ef5e-113">Вместо этого используйте **рискевенттипе** .</span><span class="sxs-lookup"><span data-stu-id="0ef5e-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="0ef5e-114">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="0ef5e-114">riskEventType</span></span>|<span data-ttu-id="0ef5e-115">string</span><span class="sxs-lookup"><span data-stu-id="0ef5e-115">string</span></span>|<span data-ttu-id="0ef5e-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="0ef5e-116">The type of risk event detected.</span></span> <span data-ttu-id="0ef5e-117">Возможные значения:,,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` и `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="0ef5e-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="0ef5e-118">описаны</span><span class="sxs-lookup"><span data-stu-id="0ef5e-118">detail</span></span>     | <span data-ttu-id="0ef5e-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0ef5e-119">riskDetail</span></span>  | <span data-ttu-id="0ef5e-120">Возможные значения:,,,,,,,,,, `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="0ef5e-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0ef5e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ef5e-121">JSON representation</span></span>

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
