---
title: Настройка области обзора доступа с помощью API microsoft Graph
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для просмотра доступа к ресурсам Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 731ebcb9ab27baf4ea30553d4f6a598d61e37d59
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010193"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Настройка области обзора доступа с помощью API microsoft Graph

API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

> [!NOTE]
> API [обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) доступен только в конечной точке Graph Microsoft. Не используйте его в производственных приложениях, так как оно может изменяться без уведомления.

Ресурсы для проверки настроены в свойстве **области** доступа к [ресурсу accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) Это свойство имеет тип [accessReviewScope](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true), абстрактный тип, унаследованный следующими ресурсами, которые можно использовать для настройки ресурсов или групп ресурсов, доступ к которые будут рассмотрены.

|Ресурс|Описание|Примеры сценариев|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)|Наиболее применимо при просмотре полного набора или подмножества директоров, имеющих доступ к ресурсу или группе связанных ресурсов.|<ul><li>Членство пользователей, назначенных группе.</li><li>Гостевой доступ пользователя к одной группе.</li><li>Гостевой доступ пользователей ко всем Microsoft 365 группам в клиенте.</li><li>Директорам служб назначены привилегированные роли.</li><li>Основной доступ пользователей и служб к пакетам доступа к управлению правами.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope?view=graph-rest-beta&preserve-view=true)|Наследуется от accessReviewQueryScope. Используется при просмотре только неактивных пользователей. Их неактивное состояние указывается **свойством inactiveDuration.** |<ul><li>Членство в группе только неактивных пользователей.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope?view=graph-rest-beta&preserve-view=true)|Наиболее применимо для проверки доступа директоров к ресурсам, в которых настраиваются уникальные пулы директоров и ресурсов.|<ul><li>Просмотр доступа к 3 определенным директорам в 1 Microsoft 365 *и* 1 привилегированной роли Azure AD.</li><ul>|

В этой статье вы будете использовать эти типы accessReviewScope для настройки широкого спектра ресурсов Azure AD в качестве области обзора доступа. Это поможет вам автоматизировать упреждающий обзор и сохранить контроль над доступом к ресурсам в организации.  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>Используйте accessReviewQueryScope для настройки области

Чтобы настроить область с помощью **типа accessReviewQueryScope,** установите значения его **запросов,** **queryRoot** и **queryType** свойств. Описание этих свойств см. в виде [ресурса accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)

### <a name="example-1-review-all-users-assigned-to-a-group"></a>Пример 1. Просмотр всех пользователей, назначенных группе

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
Чтобы *просмотреть только неактивных пользователей,* назначенных группе:

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a>Пример 2. Просмотр гостевых пользователей, назначенных группе

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a>Пример 3. Просмотр гостевых пользователей, присвоенных всем Microsoft 365 группам

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

Поскольку этот обзор применяется во всех Microsoft 365 группах, настройте **экземплярEnumerationScope,** чтобы указать Microsoft 365 группы для проверки.

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a>Пример 4. Просмотр доступа всех неактивных гостевых пользователей ко всем группам

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Поскольку этот обзор применяется к неактивным пользователям, используйте ресурс **accessReviewInactiveUsersQueryScope** и укажите свойство **типа @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` .

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a>Пример 5. Обзор всех неактивных гостевых пользователей, назначенных всем группам

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

Поскольку этот обзор применяется для всех групп, настройте **свойство instanceEnumerationScope,** чтобы указать все группы.

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a>Пример 6. Обзор назначения пакета доступа к управлению правами

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a>Пример 7. Обзор принципов служб, присвоенных привилегированным ролям 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>Для настройки области используйте principalResourceMembershipsScope

**PrincipalResourceMembershipsScope** предоставляет свойства **principalScopes** и **resourceScopes** для поддержки более адаптированных параметров конфигурации для области **accessReviewScheduleDefinition**. Это включает обзор доступа нескольких директоров или групп директоров к нескольким ресурсам.

### <a name="example-1-review-access-of-all-inactive-guest-users-to-groups"></a>Пример 1. Просмотр доступа всех неактивных гостевых пользователей к группам

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

В этом примере все директора являются неактивными гостевых пользователей с периодом их неактивности, рассчитанным в течение 30 дней с даты начала экземпляра проверки доступа.

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a>Пример 2. Просмотр доступа всех гостевых пользователей к роли каталога

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

## <a name="see-also"></a>См. также

+ [Назначение рецензентов определению проверки доступа](/graph/accessreviews-reviewers-concept)