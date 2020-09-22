---
title: Тип ресурса Рискусерактивити
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ecfe618a8db9f03bbf088ea053476fe6e51bcbf7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988942"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="8d892-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="8d892-103">riskUserActivity resource type</span></span>

<span data-ttu-id="8d892-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d892-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="8d892-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d892-105">Properties</span></span>

| <span data-ttu-id="8d892-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d892-106">Property</span></span>       | <span data-ttu-id="8d892-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8d892-107">Type</span></span>    |<span data-ttu-id="8d892-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d892-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d892-109">евенттипес</span><span class="sxs-lookup"><span data-stu-id="8d892-109">eventTypes</span></span> | <span data-ttu-id="8d892-110">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="8d892-110">riskEventType collection</span></span> |<span data-ttu-id="8d892-111">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="8d892-111">List of risk event types.</span></span> <span data-ttu-id="8d892-112">Устарело.</span><span class="sxs-lookup"><span data-stu-id="8d892-112">Deprecated.</span></span> <span data-ttu-id="8d892-113">Вместо этого используйте **рискевенттипе** .</span><span class="sxs-lookup"><span data-stu-id="8d892-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="8d892-114">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="8d892-114">riskEventType</span></span>|<span data-ttu-id="8d892-115">string</span><span class="sxs-lookup"><span data-stu-id="8d892-115">string</span></span>|<span data-ttu-id="8d892-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="8d892-116">The type of risk event detected.</span></span> <span data-ttu-id="8d892-117">Возможные значения:,,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` и `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="8d892-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="8d892-118">описаны</span><span class="sxs-lookup"><span data-stu-id="8d892-118">detail</span></span>     | <span data-ttu-id="8d892-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8d892-119">riskDetail</span></span>  | <span data-ttu-id="8d892-120">Возможные значения:,,,,,,,,,, `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="8d892-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8d892-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d892-121">JSON representation</span></span>

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


