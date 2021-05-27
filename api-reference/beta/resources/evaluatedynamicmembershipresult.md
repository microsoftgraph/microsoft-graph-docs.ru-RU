---
title: оценка типа ресурсаDynamicMembershipResult
description: Представляет результат оценки членства.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 52621ee317183a59da418ecd35309cacc0637ae3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682644"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="606dd-103">оценка типа ресурсаDynamicMembershipResult</span><span class="sxs-lookup"><span data-stu-id="606dd-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="606dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="606dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="606dd-105">Представляет результат оценки членства.</span><span class="sxs-lookup"><span data-stu-id="606dd-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="606dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="606dd-106">Properties</span></span>

| <span data-ttu-id="606dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="606dd-107">Property</span></span> | <span data-ttu-id="606dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="606dd-108">Type</span></span> | <span data-ttu-id="606dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="606dd-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="606dd-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="606dd-110">membershipRule</span></span> | <span data-ttu-id="606dd-111">String</span><span class="sxs-lookup"><span data-stu-id="606dd-111">String</span></span> | <span data-ttu-id="606dd-112">Если предоставляется групповой ID, значением является правило членства для группы.</span><span class="sxs-lookup"><span data-stu-id="606dd-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="606dd-113">Если групповой ID не предоставлен, значением является правило членства, которое было предоставлено в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="606dd-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="606dd-114">Дополнительные сведения см. в [программе Dynamic membership rules for groups in Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership)</span><span class="sxs-lookup"><span data-stu-id="606dd-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="606dd-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="606dd-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="606dd-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="606dd-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="606dd-117">Предоставляет подробный анализ результатов оценки членства.</span><span class="sxs-lookup"><span data-stu-id="606dd-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="606dd-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="606dd-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="606dd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="606dd-119">Boolean</span></span> | <span data-ttu-id="606dd-120">Значение, `true` если пользователь или устройство является членом группы.</span><span class="sxs-lookup"><span data-stu-id="606dd-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="606dd-121">Значение также может быть, если было предоставлено правило членства и пользователь или устройство проходит оценку `true` правила; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="606dd-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="606dd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="606dd-122">JSON representation</span></span>

<span data-ttu-id="606dd-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="606dd-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult",
  "baseType": null
}-->

```json
{
  "membershipRule": "String",
  "membershipRuleEvaluationDetails": {"@odata.type": "microsoft.graph.expressionEvaluationDetails"},
  "membershipRuleEvaluationResult": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "evaluateDynamicMembershipResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->