---
title: Назначение рецензентов для проверки доступа с помощью API Graph Microsoft
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 656541211226f133045a7cdbf74a72b4bcd8c369
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060516"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="0030b-103">Назначение рецензентов для проверки доступа с помощью API Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="0030b-103">Assign reviewers to your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="0030b-104">API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0030b-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

<span data-ttu-id="0030b-105">Основные рецензенты настроены в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition)</span><span class="sxs-lookup"><span data-stu-id="0030b-105">The primary reviewers are configured in the **reviewers** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) resource.</span></span>  <span data-ttu-id="0030b-106">Кроме того, вы можете указать рецензенты откатов с помощью **свойства fallbackReviewers.**</span><span class="sxs-lookup"><span data-stu-id="0030b-106">In addition, you can specify fallback reviewers by using **fallbackReviewers** property.</span></span> <span data-ttu-id="0030b-107">Эти свойства не требуются при создании самообзора (когда пользователи просматривают собственный доступ).</span><span class="sxs-lookup"><span data-stu-id="0030b-107">These properties are not required when you create a self-review (where users review their own access).</span></span>

## <a name="configure-reviewers"></a><span data-ttu-id="0030b-108">Настройка рецензентов</span><span class="sxs-lookup"><span data-stu-id="0030b-108">Configure reviewers</span></span>

<span data-ttu-id="0030b-109">Чтобы настроить рецензентов и рецензентов, задайте значения **запросов,** **queryRoot** и **queryType** свойств **accessReviewReviewerScope**.</span><span class="sxs-lookup"><span data-stu-id="0030b-109">To configure the reviewers and fallback reviewers, set the values of **query**, **queryRoot**, and **queryType** properties of **accessReviewReviewerScope**.</span></span> <span data-ttu-id="0030b-110">Описание этих свойств см. в виде [ресурса accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope)</span><span class="sxs-lookup"><span data-stu-id="0030b-110">For descriptions of these properties, see [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) resource type.</span></span>

### <a name="example-1-a-specific-user-as-the-reviewer"></a><span data-ttu-id="0030b-111">Пример 1. Конкретный пользователь в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="0030b-111">Example 1: A specific user as the reviewer</span></span>

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a><span data-ttu-id="0030b-112">Пример 2. Члены группы в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="0030b-112">Example 2: Members of a group as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a><span data-ttu-id="0030b-113">Пример 3. Владельцы групп в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="0030b-113">Example 3: Group owners as reviewers</span></span>
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

<span data-ttu-id="0030b-114">Назначение только владельцев групп из определенной страны в качестве рецензентов:</span><span class="sxs-lookup"><span data-stu-id="0030b-114">To assign only the group owners from a specific country as reviewers:</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a><span data-ttu-id="0030b-115">Пример 4. Менеджеры людей в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="0030b-115">Example 4: People managers as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
<span data-ttu-id="0030b-116">Поскольку `./manager` это относительный запрос, укажите **свойство queryRoot** со значением `decisions` .</span><span class="sxs-lookup"><span data-stu-id="0030b-116">Because `./manager` is a relative query, specify the **queryRoot** property with the value `decisions`.</span></span>

## <a name="see-also"></a><span data-ttu-id="0030b-117">См. также</span><span class="sxs-lookup"><span data-stu-id="0030b-117">See also</span></span>

+ [<span data-ttu-id="0030b-118">Настройка области определения обзора доступа</span><span class="sxs-lookup"><span data-stu-id="0030b-118">Configure the scope of your access review definition</span></span>](/graph/accessreviews-scope-concept)
