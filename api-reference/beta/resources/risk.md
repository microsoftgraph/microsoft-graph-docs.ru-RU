---
title: Тип ресурса риска
description: Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.
ms.openlocfilehash: bc8ea5c30f78560ae8750e7750596f282feb4825
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077416"
---
# <a name="risk-resource-type"></a><span data-ttu-id="28e9b-103">Тип ресурса риска</span><span class="sxs-lookup"><span data-stu-id="28e9b-103">risk resource type</span></span>

> <span data-ttu-id="28e9b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="28e9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28e9b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28e9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28e9b-106">Объединяет уровень риска, состоянии риска и сведений о риска для рискованный пользователя вход или риска события.</span><span class="sxs-lookup"><span data-stu-id="28e9b-106">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="28e9b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="28e9b-107">Properties</span></span>

| <span data-ttu-id="28e9b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="28e9b-108">Property</span></span>   | <span data-ttu-id="28e9b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="28e9b-109">Type</span></span>|<span data-ttu-id="28e9b-110">Description</span><span class="sxs-lookup"><span data-stu-id="28e9b-110">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="28e9b-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="28e9b-111">riskDetail</span></span>|<span data-ttu-id="28e9b-112">Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="28e9b-112">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="28e9b-113">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28e9b-113">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="28e9b-114">Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="28e9b-114">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="28e9b-115">riskLevel</span><span class="sxs-lookup"><span data-stu-id="28e9b-115">riskLevel</span></span>|<span data-ttu-id="28e9b-116">Предоставляет общий уровень риска рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="28e9b-116">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="28e9b-117">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28e9b-117">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="28e9b-118">Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28e9b-118">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="28e9b-119">riskLeve</span><span class="sxs-lookup"><span data-stu-id="28e9b-119">riskLeve</span></span>|<span data-ttu-id="28e9b-120">Обеспечивает уровень риска входа в при входе в систему (то есть на основании события рисков в режиме реального времени).</span><span class="sxs-lookup"><span data-stu-id="28e9b-120">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="28e9b-121">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28e9b-121">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="28e9b-122">Значение `hidden` означает, что входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28e9b-122">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="28e9b-123">riskState</span><span class="sxs-lookup"><span data-stu-id="28e9b-123">riskState</span></span>|<span data-ttu-id="28e9b-124">Предоставляет «состояние риска» рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="28e9b-124">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="28e9b-125">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28e9b-125">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28e9b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28e9b-126">JSON representation</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
