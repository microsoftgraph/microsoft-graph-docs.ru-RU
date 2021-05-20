---
title: Назначение рецензентов определению обзора доступа с помощью API Graph Microsoft
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f892e74f5bf7a7aa934872186208e21ede19780a
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579870"
---
# <a name="assign-reviewers-to-your-access-review-definition-using-the-microsoft-graph-api"></a><span data-ttu-id="a52c8-103">Назначение рецензентов определению обзора доступа с помощью API Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="a52c8-103">Assign reviewers to your access review definition using the Microsoft Graph API</span></span>

<span data-ttu-id="a52c8-104">API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a52c8-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

> [!NOTE]
> <span data-ttu-id="a52c8-105">API [обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) в настоящее время доступен только в конечной точке Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a52c8-105">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) is currently available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="a52c8-106">Не используйте его в производственных приложениях, так как оно может изменяться без уведомления.</span><span class="sxs-lookup"><span data-stu-id="a52c8-106">Do not use it in production apps, as it is subject to change without notice.</span></span>

<span data-ttu-id="a52c8-107">Основные рецензенты настроены в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="a52c8-107">The primary reviewers are configured in the **reviewers** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) resource.</span></span>  <span data-ttu-id="a52c8-108">Кроме того, вы можете указать рецензенты откатов с помощью **свойства fallbackReviewers.**</span><span class="sxs-lookup"><span data-stu-id="a52c8-108">In addition, you can specify fallback reviewers by using **fallbackReviewers** property.</span></span> <span data-ttu-id="a52c8-109">Эти свойства не требуются при создании самообзора (когда пользователи просматривают собственный доступ).</span><span class="sxs-lookup"><span data-stu-id="a52c8-109">These properties are not required when you create a self-review (where users review their own access).</span></span>

## <a name="configure-reviewers"></a><span data-ttu-id="a52c8-110">Настройка рецензентов</span><span class="sxs-lookup"><span data-stu-id="a52c8-110">Configure reviewers</span></span>

<span data-ttu-id="a52c8-111">Чтобы настроить рецензентов и рецензентов, задайте значения **запросов,** **queryRoot** и **queryType** свойств **accessReviewReviewerScope**.</span><span class="sxs-lookup"><span data-stu-id="a52c8-111">To configure the reviewers and fallback reviewers, set the values of **query**, **queryRoot**, and **queryType** properties of **accessReviewReviewerScope**.</span></span> <span data-ttu-id="a52c8-112">Описание этих свойств см. в виде [ресурса accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="a52c8-112">For descriptions of these properties, see [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true) resource type.</span></span>

### <a name="example-1-a-specific-user-as-the-reviewer"></a><span data-ttu-id="a52c8-113">Пример 1. Конкретный пользователь в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="a52c8-113">Example 1: A specific user as the reviewer</span></span>

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a><span data-ttu-id="a52c8-114">Пример 2. Члены группы в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="a52c8-114">Example 2: Members of a group as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a><span data-ttu-id="a52c8-115">Пример 3. Владельцы групп в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="a52c8-115">Example 3: Group owners as reviewers</span></span>
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

<span data-ttu-id="a52c8-116">Назначение только владельцев групп из определенной страны в качестве рецензентов:</span><span class="sxs-lookup"><span data-stu-id="a52c8-116">To assign only the group owners from a specific country as reviewers:</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a><span data-ttu-id="a52c8-117">Пример 4. Менеджеры людей в качестве рецензентов</span><span class="sxs-lookup"><span data-stu-id="a52c8-117">Example 4: People managers as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
<span data-ttu-id="a52c8-118">Поскольку `./manager` это относительный запрос, укажите **свойство queryRoot** со значением `decisions` .</span><span class="sxs-lookup"><span data-stu-id="a52c8-118">Because `./manager` is a relative query, specify the **queryRoot** property with the value `decisions`.</span></span>

## <a name="see-also"></a><span data-ttu-id="a52c8-119">См. также</span><span class="sxs-lookup"><span data-stu-id="a52c8-119">See also</span></span>

+ [<span data-ttu-id="a52c8-120">Настройка области определения обзора доступа</span><span class="sxs-lookup"><span data-stu-id="a52c8-120">Configure the scope of your access review definition</span></span>](/graph/accessreviews-scope-concept)
