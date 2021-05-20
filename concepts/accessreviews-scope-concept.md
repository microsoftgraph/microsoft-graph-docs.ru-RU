---
title: Настройка области определения обзора доступа с помощью API microsoft Graph
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для просмотра доступа к ресурсам Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: eff1d141d5c03190df4acedf7c3ed428d4cb24cd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579865"
---
# <a name="configure-the-scope-of-your-access-review-definition-using-the-microsoft-graph-api"></a><span data-ttu-id="3e981-103">Настройка области определения обзора доступа с помощью API microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3e981-103">Configure the scope of your access review definition using the Microsoft Graph API</span></span>

<span data-ttu-id="3e981-104">API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e981-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

> [!NOTE]
> <span data-ttu-id="3e981-105">API [обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) доступен только в конечной точке Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3e981-105">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) is available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="3e981-106">Не используйте его в производственных приложениях, так как оно может изменяться без уведомления.</span><span class="sxs-lookup"><span data-stu-id="3e981-106">Do not use it in production apps, as it is subject to change without notice.</span></span>

<span data-ttu-id="3e981-107">Ресурсы для проверки настроены в свойстве **области** доступа к [ресурсу accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="3e981-107">The resources to review are configured in the **scope** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) resource.</span></span> <span data-ttu-id="3e981-108">Это свойство имеет тип [accessReviewScope](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true), абстрактный тип, унаследованный следующими ресурсами, которые можно использовать для настройки ресурсов или групп ресурсов, доступ к которые будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="3e981-108">This property is of the type [accessReviewScope](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true), an abstract type inherited by the following resources that can be used to configure resources or groups of resources that access will be reviewed against.</span></span>

|<span data-ttu-id="3e981-109">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3e981-109">Resource</span></span>|<span data-ttu-id="3e981-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e981-110">Description</span></span>|<span data-ttu-id="3e981-111">Примеры сценариев</span><span class="sxs-lookup"><span data-stu-id="3e981-111">Example scenarios</span></span>|
|:---    |:---       |:---             |
|[<span data-ttu-id="3e981-112">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="3e981-112">accessReviewQueryScope</span></span>](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="3e981-113">Наиболее применимо при просмотре полного набора или подмножества директоров, имеющих доступ к ресурсу или группе связанных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3e981-113">Best applicable when reviewing the full set or subset of principals who have access to a resource or group of related resources.</span></span>|<ul><li><span data-ttu-id="3e981-114">Членство пользователей, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="3e981-114">Membership of users assigned to a group.</span></span></li><li><span data-ttu-id="3e981-115">Гостевой доступ пользователя к одной группе.</span><span class="sxs-lookup"><span data-stu-id="3e981-115">Guest user access to one group.</span></span></li><li><span data-ttu-id="3e981-116">Гостевой доступ пользователей ко всем Microsoft 365 группам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3e981-116">Guest user access to all Microsoft 365 groups in a tenant.</span></span></li><li><span data-ttu-id="3e981-117">Директорам служб назначены привилегированные роли.</span><span class="sxs-lookup"><span data-stu-id="3e981-117">Service principals assigned to privileged roles.</span></span></li><li><span data-ttu-id="3e981-118">Основной доступ пользователей и служб к пакетам доступа к управлению правами.</span><span class="sxs-lookup"><span data-stu-id="3e981-118">User and service principal access to Entitlement Management access packages.</span></span></li></ul>|
|[<span data-ttu-id="3e981-119">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="3e981-119">accessReviewInactiveUsersQueryScope</span></span>](/graph/api/resources/accessreviewinactiveusersqueryscope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="3e981-120">Наследуется от accessReviewQueryScope.</span><span class="sxs-lookup"><span data-stu-id="3e981-120">Inherited from accessReviewQueryScope.</span></span> <span data-ttu-id="3e981-121">Используется при просмотре только неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3e981-121">Used when only inactive users are reviewed.</span></span> <span data-ttu-id="3e981-122">Их неактивное состояние указывается **свойством inactiveDuration.**</span><span class="sxs-lookup"><span data-stu-id="3e981-122">Their inactive status is specified by the **inactiveDuration** property.</span></span> |<ul><li><span data-ttu-id="3e981-123">Членство в группе только неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3e981-123">Group membership of only inactive users.</span></span></li><ul>|
|[<span data-ttu-id="3e981-124">principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="3e981-124">principalResourceMembershipsScope</span></span>](/graph/api/resources/principalResourceMembershipsScope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="3e981-125">Наиболее применимо для проверки доступа директоров к ресурсам, в которых настраиваются уникальные пулы директоров и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3e981-125">Best applicable to review principals' access to resources where you configure unique pools of principals and resources.</span></span>|<ul><li><span data-ttu-id="3e981-126">Просмотр доступа к 3 определенным директорам в 1 Microsoft 365 *и* 1 привилегированной роли Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e981-126">Reviewing access of 3 specific principals across 1 Microsoft 365 group *and* 1 privileged Azure AD role.</span></span></li><ul>|

<span data-ttu-id="3e981-127">В этой статье вы будете использовать эти типы accessReviewScope для настройки широкого спектра ресурсов Azure AD в качестве области обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="3e981-127">In this article, you will use these types of accessReviewScope to configure a wide range of Azure AD resources as the scope of your access review.</span></span> <span data-ttu-id="3e981-128">Это поможет вам автоматизировать упреждающий обзор и сохранить контроль над доступом к ресурсам в организации.</span><span class="sxs-lookup"><span data-stu-id="3e981-128">This can help you to automate proactive review and keep control over access to resources in your organization.</span></span>  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a><span data-ttu-id="3e981-129">Используйте accessReviewQueryScope для настройки области</span><span class="sxs-lookup"><span data-stu-id="3e981-129">Use accessReviewQueryScope to configure scope</span></span>

<span data-ttu-id="3e981-130">Чтобы настроить область с помощью **типа accessReviewQueryScope,** установите значения его **запросов,** **queryRoot** и **queryType** свойств.</span><span class="sxs-lookup"><span data-stu-id="3e981-130">To configure the scope by using the **accessReviewQueryScope** type, set the values of its **query**, **queryRoot**, and **queryType** properties.</span></span> <span data-ttu-id="3e981-131">Описание этих свойств см. в виде [ресурса accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="3e981-131">For descriptions of these properties, see [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true) resource type.</span></span>

### <a name="example-1-review-all-users-assigned-to-a-group"></a><span data-ttu-id="3e981-132">Пример 1. Просмотр всех пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="3e981-132">Example 1: Review all users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
<span data-ttu-id="3e981-133">Чтобы *просмотреть только неактивных пользователей,* назначенных группе:</span><span class="sxs-lookup"><span data-stu-id="3e981-133">To review *only inactive users* assigned to the group:</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a><span data-ttu-id="3e981-134">Пример 2. Просмотр гостевых пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="3e981-134">Example 2: Review guest users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a><span data-ttu-id="3e981-135">Пример 3. Просмотр гостевых пользователей, присвоенных всем Microsoft 365 группам</span><span class="sxs-lookup"><span data-stu-id="3e981-135">Example 3: Review guest users assigned to all Microsoft 365 groups</span></span>

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

<span data-ttu-id="3e981-136">Поскольку этот обзор применяется во всех Microsoft 365 группах, настройте **экземплярEnumerationScope,** чтобы указать Microsoft 365 группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="3e981-136">Because this review is applied on all Microsoft 365 groups, configure the **instanceEnumerationScope** to specify the Microsoft 365 groups to review.</span></span>

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a><span data-ttu-id="3e981-137">Пример 4. Просмотр доступа всех неактивных гостевых пользователей ко всем группам</span><span class="sxs-lookup"><span data-stu-id="3e981-137">Example 4: Review access of all inactive guest users to all groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="3e981-138">Поскольку этот обзор применяется к неактивным пользователям, используйте ресурс **accessReviewInactiveUsersQueryScope** и укажите свойство **типа @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` .</span><span class="sxs-lookup"><span data-stu-id="3e981-138">Because this review is applied on inactive users, use the **accessReviewInactiveUsersQueryScope** resource and specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span>

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a><span data-ttu-id="3e981-139">Пример 5. Обзор всех неактивных гостевых пользователей, назначенных всем группам</span><span class="sxs-lookup"><span data-stu-id="3e981-139">Example 5: Review of all inactive guest users assigned to all teams</span></span>

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

<span data-ttu-id="3e981-140">Поскольку этот обзор применяется для всех групп, настройте **свойство instanceEnumerationScope,** чтобы указать все группы.</span><span class="sxs-lookup"><span data-stu-id="3e981-140">Because this review is applied on all teams, configure the **instanceEnumerationScope** property to specify all teams.</span></span>

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a><span data-ttu-id="3e981-141">Пример 6. Обзор назначения пакета доступа к управлению правами</span><span class="sxs-lookup"><span data-stu-id="3e981-141">Example 6: Review of Entitlement Management access package assignment</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a><span data-ttu-id="3e981-142">Пример 7. Обзор принципов служб, присвоенных привилегированным ролям</span><span class="sxs-lookup"><span data-stu-id="3e981-142">Example 7: Review of service principals assigned to privileged roles</span></span> 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a><span data-ttu-id="3e981-143">Для настройки области используйте principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="3e981-143">Use principalResourceMembershipsScope to configure scope</span></span>

<span data-ttu-id="3e981-144">**PrincipalResourceMembershipsScope** предоставляет свойства **principalScopes** и **resourceScopes** для поддержки более адаптированных параметров конфигурации для области **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="3e981-144">The **principalResourceMembershipsScope** exposes the **principalScopes** and **resourceScopes** properties to support more tailored configuration options for the scope of the **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="3e981-145">Это включает обзор доступа нескольких директоров или групп директоров к нескольким ресурсам.</span><span class="sxs-lookup"><span data-stu-id="3e981-145">This includes reviewing access for multiple principals or groups of principals to multiple resources.</span></span>

### <a name="example-1-review-access-of-all-inactive-guest-users-to-an-application"></a><span data-ttu-id="3e981-146">Пример 1. Просмотр доступа всех неактивных гостевых пользователей к приложению</span><span class="sxs-lookup"><span data-stu-id="3e981-146">Example 1: Review access of all inactive guest users to an application</span></span>

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
            "query": "/servicePrincipals/{serviceprincipal id}",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

<span data-ttu-id="3e981-147">В этом примере все директора являются неактивными гостевых пользователей с периодом их неактивности, рассчитанным в течение 30 дней с даты начала экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="3e981-147">In this example, the principals are all inactive guest users with the period of their inactivity calculated as 30 days from the start date of the access review instance.</span></span>

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a><span data-ttu-id="3e981-148">Пример 2. Просмотр доступа всех гостевых пользователей к роли каталога</span><span class="sxs-lookup"><span data-stu-id="3e981-148">Example 2: Review access of all guest users to a directory role</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3e981-149">См. также</span><span class="sxs-lookup"><span data-stu-id="3e981-149">See also</span></span>

+ [<span data-ttu-id="3e981-150">Назначение рецензентов определению проверки доступа</span><span class="sxs-lookup"><span data-stu-id="3e981-150">Assign reviewers to your access review definition</span></span>](/graph/accessreviews-reviewers-concept)