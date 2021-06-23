---
title: Настройка области обзора доступа с помощью API microsoft Graph
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для просмотра доступа к ресурсам Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: a4ed9b17d8d2b831071dc8f24e8330e595b543dc
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060291"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="27b58-103">Настройка области обзора доступа с помощью API microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b58-103">Configure the scope of your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="27b58-104">API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27b58-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

<span data-ttu-id="27b58-105">Ресурсы для проверки настроены в свойстве **области** доступа к [ресурсу accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition)</span><span class="sxs-lookup"><span data-stu-id="27b58-105">The resources to review are configured in the **scope** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) resource.</span></span> <span data-ttu-id="27b58-106">Это свойство имеет тип [accessReviewScope](/graph/api/resources/accessreviewscope), абстрактный тип, унаследованный следующими ресурсами, которые можно использовать для настройки ресурсов или групп ресурсов, доступ к которые будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="27b58-106">This property is of the type [accessReviewScope](/graph/api/resources/accessreviewscope), an abstract type inherited by the following resources that can be used to configure resources or groups of resources that access will be reviewed against.</span></span>

|<span data-ttu-id="27b58-107">Ресурс</span><span class="sxs-lookup"><span data-stu-id="27b58-107">Resource</span></span>|<span data-ttu-id="27b58-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27b58-108">Description</span></span>|<span data-ttu-id="27b58-109">Примеры сценариев</span><span class="sxs-lookup"><span data-stu-id="27b58-109">Example scenarios</span></span>|
|:---    |:---       |:---             |
|[<span data-ttu-id="27b58-110">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="27b58-110">accessReviewQueryScope</span></span>](/graph/api/resources/accessreviewqueryscope)|<span data-ttu-id="27b58-111">Наиболее применимо при просмотре полного набора или подмножества директоров, имеющих доступ к ресурсу или группе связанных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="27b58-111">Best applicable when reviewing the full set or subset of principals who have access to a resource or group of related resources.</span></span>|<ul><li><span data-ttu-id="27b58-112">Членство пользователей, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="27b58-112">Membership of users assigned to a group.</span></span></li><li><span data-ttu-id="27b58-113">Гостевой доступ пользователя к одной группе.</span><span class="sxs-lookup"><span data-stu-id="27b58-113">Guest user access to one group.</span></span></li><li><span data-ttu-id="27b58-114">Гостевой доступ пользователей ко всем Microsoft 365 группам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="27b58-114">Guest user access to all Microsoft 365 groups in a tenant.</span></span></li><li><span data-ttu-id="27b58-115">Директорам служб назначены привилегированные роли.</span><span class="sxs-lookup"><span data-stu-id="27b58-115">Service principals assigned to privileged roles.</span></span></li><li><span data-ttu-id="27b58-116">Основной доступ пользователей и служб к пакетам доступа к управлению правами.</span><span class="sxs-lookup"><span data-stu-id="27b58-116">User and service principal access to Entitlement Management access packages.</span></span></li></ul>|
|[<span data-ttu-id="27b58-117">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="27b58-117">accessReviewInactiveUsersQueryScope</span></span>](/graph/api/resources/accessreviewinactiveusersqueryscope)|<span data-ttu-id="27b58-118">Наследуется от accessReviewQueryScope.</span><span class="sxs-lookup"><span data-stu-id="27b58-118">Inherited from accessReviewQueryScope.</span></span> <span data-ttu-id="27b58-119">Используется при просмотре только неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="27b58-119">Used when only inactive users are reviewed.</span></span> <span data-ttu-id="27b58-120">Их неактивное состояние указывается **свойством inactiveDuration.**</span><span class="sxs-lookup"><span data-stu-id="27b58-120">Their inactive status is specified by the **inactiveDuration** property.</span></span> |<ul><li><span data-ttu-id="27b58-121">Членство в группе только неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="27b58-121">Group membership of only inactive users.</span></span></li><ul>|
|[<span data-ttu-id="27b58-122">principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="27b58-122">principalResourceMembershipsScope</span></span>](/graph/api/resources/principalResourceMembershipsScope)|<span data-ttu-id="27b58-123">Наиболее применимо для проверки доступа директоров к ресурсам, в которых настраиваются уникальные пулы директоров и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="27b58-123">Best applicable to review principals' access to resources where you configure unique pools of principals and resources.</span></span>|<ul><li><span data-ttu-id="27b58-124">Просмотр доступа к 3 определенным директорам в 1 Microsoft 365 *и* 1 привилегированной роли Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27b58-124">Reviewing access of 3 specific principals across 1 Microsoft 365 group *and* 1 privileged Azure AD role.</span></span></li><ul>|

<span data-ttu-id="27b58-125">В этой статье вы будете использовать эти типы accessReviewScope для настройки широкого спектра ресурсов Azure AD в качестве области обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="27b58-125">In this article, you will use these types of accessReviewScope to configure a wide range of Azure AD resources as the scope of your access review.</span></span> <span data-ttu-id="27b58-126">Это поможет вам автоматизировать упреждающий обзор и сохранить контроль над доступом к ресурсам в организации.</span><span class="sxs-lookup"><span data-stu-id="27b58-126">This can help you to automate proactive review and keep control over access to resources in your organization.</span></span>  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a><span data-ttu-id="27b58-127">Используйте accessReviewQueryScope для настройки области</span><span class="sxs-lookup"><span data-stu-id="27b58-127">Use accessReviewQueryScope to configure scope</span></span>

<span data-ttu-id="27b58-128">Чтобы настроить область с помощью **типа accessReviewQueryScope,** установите значения его **запросов,** **queryRoot** и **queryType** свойств.</span><span class="sxs-lookup"><span data-stu-id="27b58-128">To configure the scope by using the **accessReviewQueryScope** type, set the values of its **query**, **queryRoot**, and **queryType** properties.</span></span> <span data-ttu-id="27b58-129">Описание этих свойств см. в виде [ресурса accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope)</span><span class="sxs-lookup"><span data-stu-id="27b58-129">For descriptions of these properties, see [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) resource type.</span></span>

### <a name="example-1-review-all-users-assigned-to-a-group"></a><span data-ttu-id="27b58-130">Пример 1. Просмотр всех пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="27b58-130">Example 1: Review all users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
<span data-ttu-id="27b58-131">Чтобы *просмотреть только неактивных пользователей,* назначенных группе:</span><span class="sxs-lookup"><span data-stu-id="27b58-131">To review *only inactive users* assigned to the group:</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a><span data-ttu-id="27b58-132">Пример 2. Просмотр гостевых пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="27b58-132">Example 2: Review guest users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a><span data-ttu-id="27b58-133">Пример 3. Просмотр гостевых пользователей, присвоенных всем Microsoft 365 группам</span><span class="sxs-lookup"><span data-stu-id="27b58-133">Example 3: Review guest users assigned to all Microsoft 365 groups</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true ",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

<span data-ttu-id="27b58-134">Поскольку этот обзор применяется во всех Microsoft 365 группах, настройте **экземплярEnumerationScope,** чтобы указать Microsoft 365 группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="27b58-134">Because this review is applied on all Microsoft 365 groups, configure the **instanceEnumerationScope** to specify the Microsoft 365 groups to review.</span></span>

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a><span data-ttu-id="27b58-135">Пример 4. Просмотр доступа всех неактивных гостевых пользователей ко всем группам</span><span class="sxs-lookup"><span data-stu-id="27b58-135">Example 4: Review access of all inactive guest users to all groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="27b58-136">Поскольку этот обзор применяется к неактивным пользователям, используйте ресурс **accessReviewInactiveUsersQueryScope** и укажите свойство **типа @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` .</span><span class="sxs-lookup"><span data-stu-id="27b58-136">Because this review is applied on inactive users, use the **accessReviewInactiveUsersQueryScope** resource and specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span>

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a><span data-ttu-id="27b58-137">Пример 5. Обзор всех неактивных гостевых пользователей, назначенных всем группам</span><span class="sxs-lookup"><span data-stu-id="27b58-137">Example 5: Review of all inactive guest users assigned to all teams</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="27b58-138">Поскольку этот обзор применяется для всех групп, настройте **свойство instanceEnumerationScope,** чтобы указать все группы.</span><span class="sxs-lookup"><span data-stu-id="27b58-138">Because this review is applied on all teams, configure the **instanceEnumerationScope** property to specify all teams.</span></span>

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a><span data-ttu-id="27b58-139">Пример 6. Обзор назначения пакета доступа к управлению правами</span><span class="sxs-lookup"><span data-stu-id="27b58-139">Example 6: Review of Entitlement Management access package assignment</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a><span data-ttu-id="27b58-140">Пример 7. Обзор принципов служб, присвоенных привилегированным ролям</span><span class="sxs-lookup"><span data-stu-id="27b58-140">Example 7: Review of service principals assigned to privileged roles</span></span> 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a><span data-ttu-id="27b58-141">Для настройки области используйте principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="27b58-141">Use principalResourceMembershipsScope to configure scope</span></span>

<span data-ttu-id="27b58-142">**PrincipalResourceMembershipsScope** предоставляет свойства **principalScopes** и **resourceScopes** для поддержки более адаптированных параметров конфигурации для области **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="27b58-142">The **principalResourceMembershipsScope** exposes the **principalScopes** and **resourceScopes** properties to support more tailored configuration options for the scope of the **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="27b58-143">Это включает обзор доступа нескольких директоров или групп директоров к нескольким ресурсам.</span><span class="sxs-lookup"><span data-stu-id="27b58-143">This includes reviewing access for multiple principals or groups of principals to multiple resources.</span></span>

### <a name="example-1-review-access-of-all-inactive-guest-users-to-groups"></a><span data-ttu-id="27b58-144">Пример 1. Просмотр доступа всех неактивных гостевых пользователей к группам</span><span class="sxs-lookup"><span data-stu-id="27b58-144">Example 1: Review access of all inactive guest users to groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph",
            "inactiveDuration": "P30D"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

<span data-ttu-id="27b58-145">В этом примере все директора являются неактивными гостевых пользователей с периодом их неактивности, рассчитанным в течение 30 дней с даты начала экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="27b58-145">In this example, the principals are all inactive guest users with the period of their inactivity calculated as 30 days from the start date of the access review instance.</span></span>

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a><span data-ttu-id="27b58-146">Пример 2. Просмотр доступа всех гостевых пользователей к роли каталога</span><span class="sxs-lookup"><span data-stu-id="27b58-146">Example 2: Review access of all guest users to a directory role</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/roleManagement/directory/roleDefinitions/{role id}",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="27b58-147">См. также</span><span class="sxs-lookup"><span data-stu-id="27b58-147">See also</span></span>

+ [<span data-ttu-id="27b58-148">Назначение рецензентов определению проверки доступа</span><span class="sxs-lookup"><span data-stu-id="27b58-148">Assign reviewers to your access review definition</span></span>](/graph/accessreviews-reviewers-concept)
