---
title: Настройка области обзора доступа с помощью API microsoft Graph
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для просмотра доступа к ресурсам Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 268e9ce5a364e23551fd8140456ce245f6613ff75e878940feb467b9b5bd0de6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129717"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Настройка области обзора доступа с помощью API microsoft Graph

API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

Ресурсы для проверки настроены в свойстве **области** доступа к [ресурсу accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition) Это свойство имеет тип [accessReviewScope](/graph/api/resources/accessreviewscope), абстрактный тип, унаследованный следующими ресурсами, которые можно использовать для настройки ресурсов или групп ресурсов, доступ к которые будут рассмотрены.

|Ресурс|Описание|Примеры сценариев|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|Наиболее применимо при просмотре полного набора или подмножества директоров, имеющих доступ к ресурсу или группе связанных ресурсов.|<ul><li>Членство пользователей, назначенных группе.</li><li>Гостевой доступ пользователя к одной группе.</li><li>Гостевой доступ пользователей ко всем Microsoft 365 группам в клиенте.</li><li>Директорам служб назначены привилегированные роли.</li><li>Основной доступ пользователей и служб к пакетам доступа к управлению правами.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|Наследуется от accessReviewQueryScope. Используется при просмотре только неактивных пользователей. Их неактивное состояние указывается **свойством inactiveDuration.** |<ul><li>Членство в группе только неактивных пользователей.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|Наиболее применимо для проверки доступа директоров к ресурсам, в которых настраиваются уникальные пулы директоров и ресурсов.|<ul><li>Просмотр доступа к 3 определенным директорам в 1 Microsoft 365 *и* 1 привилегированной роли Azure AD.</li><ul>|

В этой статье вы будете использовать эти типы accessReviewScope для настройки широкого спектра ресурсов Azure AD в качестве области обзора доступа. Это поможет вам автоматизировать упреждающий обзор и сохранить контроль над доступом к ресурсам в организации.  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>Используйте accessReviewQueryScope для настройки области

Чтобы настроить область с помощью **типа accessReviewQueryScope,** установите значения его **запросов,** **queryRoot** и **queryType** свойств. Описание этих свойств см. в виде [ресурса accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope)

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
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
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
