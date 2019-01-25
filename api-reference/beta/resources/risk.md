---
title: Тип ресурса риска
description: Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524823"
---
# <a name="risk-resource-type"></a><span data-ttu-id="6f4ce-103">Тип ресурса риска</span><span class="sxs-lookup"><span data-stu-id="6f4ce-103">risk resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f4ce-104">Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-104">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="6f4ce-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f4ce-105">Properties</span></span>

| <span data-ttu-id="6f4ce-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f4ce-106">Property</span></span>   | <span data-ttu-id="6f4ce-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6f4ce-107">Type</span></span>|<span data-ttu-id="6f4ce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6f4ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="6f4ce-109">riskDetail</span><span class="sxs-lookup"><span data-stu-id="6f4ce-109">riskDetail</span></span>|<span data-ttu-id="6f4ce-110">Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-110">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6f4ce-111">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-111">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="6f4ce-112">Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-112">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="6f4ce-113">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6f4ce-113">riskLevel</span></span>|<span data-ttu-id="6f4ce-114">Предоставляет общий уровень риска рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-114">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6f4ce-115">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-115">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="6f4ce-116">Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-116">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="6f4ce-117">riskLeve</span><span class="sxs-lookup"><span data-stu-id="6f4ce-117">riskLeve</span></span>|<span data-ttu-id="6f4ce-118">Обеспечивает уровень риска входа в при входе в систему (то есть на основании события рисков в режиме реального времени).</span><span class="sxs-lookup"><span data-stu-id="6f4ce-118">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="6f4ce-119">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-119">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="6f4ce-120">Значение `hidden` означает, что входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-120">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="6f4ce-121">riskState</span><span class="sxs-lookup"><span data-stu-id="6f4ce-121">riskState</span></span>|<span data-ttu-id="6f4ce-122">Предоставляет «состояние риска» рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-122">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6f4ce-123">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f4ce-123">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f4ce-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f4ce-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
