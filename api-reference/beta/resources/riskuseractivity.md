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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="59dc8-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="59dc8-103">riskUserActivity resource type</span></span>

<span data-ttu-id="59dc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59dc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="59dc8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="59dc8-105">Properties</span></span>

| <span data-ttu-id="59dc8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="59dc8-106">Property</span></span>       | <span data-ttu-id="59dc8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="59dc8-107">Type</span></span>    |<span data-ttu-id="59dc8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="59dc8-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59dc8-109">евенттипес</span><span class="sxs-lookup"><span data-stu-id="59dc8-109">eventTypes</span></span> | <span data-ttu-id="59dc8-110">Коллекция Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="59dc8-110">riskEventType collection</span></span> |<span data-ttu-id="59dc8-111">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="59dc8-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="59dc8-112">описаны</span><span class="sxs-lookup"><span data-stu-id="59dc8-112">detail</span></span>     | <span data-ttu-id="59dc8-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="59dc8-113">riskDetail</span></span>  | <span data-ttu-id="59dc8-114">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="59dc8-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="59dc8-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59dc8-115">JSON representation</span></span>

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
