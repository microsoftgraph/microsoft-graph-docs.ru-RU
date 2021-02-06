---
title: Тип ресурса evaluateDynamicMembershipResult
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1df07449605f3b1d48c01b1e352100d534fc9b1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129508"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="dd44a-103">Тип ресурса evaluateDynamicMembershipResult</span><span class="sxs-lookup"><span data-stu-id="dd44a-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="dd44a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd44a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd44a-105">Представляет результат оценки членства.</span><span class="sxs-lookup"><span data-stu-id="dd44a-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="dd44a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd44a-106">Properties</span></span>

| <span data-ttu-id="dd44a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd44a-107">Property</span></span> | <span data-ttu-id="dd44a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dd44a-108">Type</span></span> | <span data-ttu-id="dd44a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dd44a-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="dd44a-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="dd44a-110">membershipRule</span></span> | <span data-ttu-id="dd44a-111">String</span><span class="sxs-lookup"><span data-stu-id="dd44a-111">String</span></span> | <span data-ttu-id="dd44a-112">Если предоставлен ИД группы, значением является правило членства для группы.</span><span class="sxs-lookup"><span data-stu-id="dd44a-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="dd44a-113">Если ид группы не предоставлен, значением является правило членства, предоставленное в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="dd44a-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="dd44a-114">Дополнительные сведения см. в правилах [динамического членства для групп в Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership)</span><span class="sxs-lookup"><span data-stu-id="dd44a-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="dd44a-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="dd44a-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="dd44a-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="dd44a-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="dd44a-117">Предоставляет подробный анализ результатов оценки членства.</span><span class="sxs-lookup"><span data-stu-id="dd44a-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="dd44a-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="dd44a-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="dd44a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd44a-119">Boolean</span></span> | <span data-ttu-id="dd44a-120">Значением `true` является, если пользователь или устройство входит в группу.</span><span class="sxs-lookup"><span data-stu-id="dd44a-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="dd44a-121">Значение также может быть, если предоставлено правило членства и пользователь или устройство проходят оценку правила; в противном `true` случае `false` .</span><span class="sxs-lookup"><span data-stu-id="dd44a-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd44a-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dd44a-122">JSON representation</span></span>

<span data-ttu-id="dd44a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd44a-123">The following is a JSON representation of the resource.</span></span>

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