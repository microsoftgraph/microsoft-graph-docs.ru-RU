---
title: Тип ресурса Евалуатединамикмембершипресулт
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a38ae33d59ea8deba8a71e48698baeddf709ae9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071238"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="c38c0-103">Тип ресурса Евалуатединамикмембершипресулт</span><span class="sxs-lookup"><span data-stu-id="c38c0-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="c38c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c38c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c38c0-105">Представляет результат оценки членства.</span><span class="sxs-lookup"><span data-stu-id="c38c0-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="c38c0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c38c0-106">Properties</span></span>

| <span data-ttu-id="c38c0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c38c0-107">Property</span></span> | <span data-ttu-id="c38c0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c38c0-108">Type</span></span> | <span data-ttu-id="c38c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c38c0-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c38c0-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="c38c0-110">membershipRule</span></span> | <span data-ttu-id="c38c0-111">String</span><span class="sxs-lookup"><span data-stu-id="c38c0-111">String</span></span> | <span data-ttu-id="c38c0-112">Если указан идентификатор группы, то значение является правилом членства для группы.</span><span class="sxs-lookup"><span data-stu-id="c38c0-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="c38c0-113">Если идентификатор группы не указан, то значением является правило членства, предоставленное в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="c38c0-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="c38c0-114">Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="c38c0-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="c38c0-115">мембершипруливалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="c38c0-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="c38c0-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="c38c0-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="c38c0-117">Предоставляет подробные анайлсис результатов оценки членства.</span><span class="sxs-lookup"><span data-stu-id="c38c0-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="c38c0-118">мембершипруливалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="c38c0-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="c38c0-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c38c0-119">Boolean</span></span> | <span data-ttu-id="c38c0-120">Значение, `true` Если пользователь или устройство является участником группы.</span><span class="sxs-lookup"><span data-stu-id="c38c0-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="c38c0-121">Значение также может быть `true` указано в том случае, если было предоставлено правило членства, и пользователь или устройство проходят оценку правила; в противном случае — значение `false` .</span><span class="sxs-lookup"><span data-stu-id="c38c0-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c38c0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c38c0-122">JSON representation</span></span>

<span data-ttu-id="c38c0-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c38c0-123">The following is a JSON representation of the resource.</span></span>

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

