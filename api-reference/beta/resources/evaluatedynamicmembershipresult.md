---
title: Тип ресурса Евалуатединамикмембершипресулт
description: Представляет результат оценки членства.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6e40c796468a8c31d2cd75dd2b6815440bfb71e
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272853"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="5b1f2-103">Тип ресурса Евалуатединамикмембершипресулт</span><span class="sxs-lookup"><span data-stu-id="5b1f2-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="5b1f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b1f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b1f2-105">Представляет результат оценки членства.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="5b1f2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b1f2-106">Properties</span></span>

| <span data-ttu-id="5b1f2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b1f2-107">Property</span></span> | <span data-ttu-id="5b1f2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b1f2-108">Type</span></span> | <span data-ttu-id="5b1f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b1f2-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="5b1f2-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="5b1f2-110">membershipRule</span></span> | <span data-ttu-id="5b1f2-111">String</span><span class="sxs-lookup"><span data-stu-id="5b1f2-111">String</span></span> | <span data-ttu-id="5b1f2-112">Если указан идентификатор группы, то значение является правилом членства для группы.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="5b1f2-113">Если идентификатор группы не указан, то значением является правило членства, предоставленное в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="5b1f2-114">Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="5b1f2-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="5b1f2-115">мембершипруливалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="5b1f2-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="5b1f2-116">експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="5b1f2-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="5b1f2-117">Предоставляет подробные анайлсис результатов оценки членства.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="5b1f2-118">мембершипруливалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="5b1f2-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="5b1f2-119">Логический</span><span class="sxs-lookup"><span data-stu-id="5b1f2-119">Boolean</span></span> | <span data-ttu-id="5b1f2-120">Значение, `true` Если пользователь или устройство является участником группы.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="5b1f2-121">Значение также может быть `true` указано в том случае, если было предоставлено правило членства, и пользователь или устройство проходят оценку правила; в противном случае — значение `false` .</span><span class="sxs-lookup"><span data-stu-id="5b1f2-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b1f2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b1f2-122">JSON representation</span></span>

<span data-ttu-id="5b1f2-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b1f2-123">The following is a JSON representation of the resource.</span></span>

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