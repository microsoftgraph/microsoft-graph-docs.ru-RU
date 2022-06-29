---
title: Настройка области проверки доступа с помощью microsoft API Graph
description: Узнайте, как программно проверить доступ пользователей, субъектов-служб или групп к Azure AD с помощью microsoft API Graph.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: cb8b96c06704a3e66eee38d729fca9a627a12896
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446219"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Настройка области проверки доступа с помощью microsoft API Graph

API Azure AD доступа позволяет [](/graph/api/resources/accessreviewsv2-overview) программно проверить доступ пользователей, субъектов-служб или групп к Azure AD ресурсам. API помогает автоматизировать упреждающий просмотр и контролировать доступ к ресурсам в организации.  

Проверяемые ресурсы настраиваются в свойстве **области** ресурса [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) . Это свойство имеет тип [accessReviewScope](/graph/api/resources/accessreviewscope), абстрактный тип, от которого наследуются следующие ресурсы API, которые можно использовать для настройки области проверки доступа.

|Ресурс|Описание|Примеры сценариев|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|Наследуется **от accessReviewScope**. Лучше всего подходит при просмотре полного набора или подмножества субъектов, имеющих доступ к ресурсу или группе связанных ресурсов.|<ul><li>Членство пользователей, назначенных группе, прямых или прямых и транзитивных участников.</li><li>Гостевой пользователь имеет доступ к одной группе.</li><li>Гостевой пользователь имеет доступ ко всем группам Microsoft 365 в клиенте.</li><li>Субъекты-службы, назначенные привилегированным ролям.</li><li>Доступ пользователя и субъекта-службы к пакетам доступа управления правами.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|Наследуется **от accessReviewQueryScope**. Используется, если проверяются только неактивные пользователи. Их состояние неактивности указывается **свойством inactiveDuration** . |<ul><li>Членство в группах только неактивных пользователей.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|Наследуется **от accessReviewScope**. Лучше всего подходит для проверки доступа субъектов к ресурсам, в которых настраиваются уникальные пулы субъектов и ресурсов.|<ul><li>Просмотр доступа трех определенных участников в одной группе Microsoft 365 и одной привилегированной Azure AD роли.</li><ul>|

В этой статье вы узнаете, как ограничить область проверки доступа с помощью этих трех производных типов ресурсов.

## <a name="use-accessreviewqueryscope-and-accessreviewinactiveusersqueryscope-to-configure-scope"></a>Использование accessReviewQueryScope и accessReviewInactiveUsersQueryScope для настройки области

Чтобы настроить область с помощью типа **accessReviewQueryScope** , задайте значения свойств запроса **,** **queryRoot** и **queryType** . Описание этих свойств см. в описании [типа ресурса accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) .

**AccessReviewInactiveUsersQueryScope** требует всех свойств **accessReviewQueryScope** и включает свойство **inactiveDuration** .

### <a name="example-1-review-all-users-assigned-to-a-group"></a>Пример 1. Просмотр всех пользователей, назначенных группе

В следующем примере проверка определяется как прямыми, так и транзитивными членами группы, которые являются пользователями. Транзитивные члены являются членами вложенных групп.

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

**Пример сценария:** Предположим, что группа A имеет трех прямых участников: пользователей AU1 и AU2 и группу G1. Группа G1, с другой стороны, имеет два члена: пользователи GU1 и GU2. Поэтому пользователи GU1 и GU2 являются транзитивными членами вложенной группы G1. В проверку будут включены четыре объекта: пользователи AU1, AU2, GU1 и GU2.

Чтобы *просмотреть только неактивных пользователей* , назначенных группе:

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

В этом примере также область проверки определяется как прямыми, так и транзитивными членами группы, которые являются неактивными пользователями.

### <a name="example-2-review-all-guest-users-assigned-to-a-group"></a>Пример 2. Просмотр всех гостевых пользователей, назначенных группе

В следующем примере проверка определяется как прямыми, так и транзитивными членами группы, которые являются гостевыми пользователями. Транзитивные члены являются членами вложенных групп.

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-all-users-and-groups-assigned-to-a-group"></a>Пример 3. Просмотр всех пользователей и групп, назначенных группе

В следующем примере проверка определяется только непосредственными участниками группы, которые являются пользователями или другими группами. В этой области:
+ В проверку включаются прямые пользователи.
+ Прямые группы включаются в проверку.
+ Транзитивные члены групп, то есть члены вложенных групп, не включаются в проверку.

```http
"scope": {
        "query": "/groups/{group id}/members",
        "queryType": "MicrosoftGraph"
}
```

**Пример сценария:** Предположим, что группа A имеет трех прямых участников: пользователей AU1 и AU2 и группу G1. Группа G1, с другой стороны, имеет два члена: пользователи GU1 и GU2. Поэтому пользователи GU1 и GU2 являются транзитивными членами вложенной группы G1. В приведенной выше проверке целевыми объектами являются только три объекта: au1 и AU2, а также группа G1.

### <a name="example-4-review-all-users-assigned-to-all-microsoft-365-groups"></a>Пример 4. Просмотр всех пользователей, назначенных всем группам Microsoft 365

В следующем примере создается проверка каждой группы Microsoft 365, содержащего гостевых пользователей. Для экземпляра проверки в каждой группе проверка применяется только к прямым участникам группы, которые являются гостевыми пользователями.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

Кроме того, так как эта проверка применяется ко всем группам Microsoft 365, настройте **instanceEnumerationScope** , чтобы указать группы Microsoft 365 для проверки. Динамические группы и группы, назначаемые ролем, не включаются в эту проверку.

### <a name="example-5-review-all-guest-users-assigned-to-all-microsoft-365-groups"></a>Пример 5. Просмотр всех гостевых пользователей, назначенных всем группам Microsoft 365

В следующем примере область проверки определяется для прямых участников всех групп Microsoft 365, которые являются гостевыми пользователями.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

Кроме того, так как эта проверка применяется ко всем группам Microsoft 365, настройте **instanceEnumerationScope** , чтобы указать группы Microsoft 365 для проверки. Динамические группы и группы, назначаемые ролем, не включаются в эту проверку.

#### <a name="review-all-inactive-guest-users-assigned-to-all-microsoft-365-groups"></a>Проверка всех неактивных гостевых пользователей, назначенных всем группам Microsoft 365

В следующем примере область проверки определяется для всех участников Microsoft 365, которые являются неактивными гостевыми пользователями.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Кроме того, поскольку эта проверка применяется к неактивным пользователям, используйте ресурс **accessReviewInactiveUsersQueryScope** и укажите свойство **@odata.type** `#microsoft.graph.accessReviewInactiveUsersQueryScope`со значением . Динамические группы и группы, назначаемые ролем, не включаются в эту проверку.

### <a name="example-6-review-all-guest-users-assigned-to-all-teams"></a>Пример 6. Просмотр всех гостевых пользователей, назначенных всем командам

В следующем примере проверка определяется для прямых участников всех команд, которые являются гостевыми пользователями.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```
    
Кроме того, поскольку эта проверка применяется ко всем группам Microsoft 365 с поддержкой Teams, настройте **instanceEnumerationScope** , чтобы указать группы Microsoft 365 с поддержкой Teams для проверки. Динамические группы и группы, назначаемые ролем, не включаются в эту проверку.

Эта проверка не будет включать пользователей прямого подключения B2B в команды с общими каналами. Чтобы включить пользователей прямого подключения B2B в команды с общими каналами, см. пример 11. Просмотр всех пользователей, назначенных команде [, включая пользователей прямого подключения B2B](#example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) в команде с общими каналами.

#### <a name="review-all-inactive-guest-users-assigned-to-all-teams"></a>Просмотр всех неактивных гостевых пользователей, назначенных всем teams

В следующем примере область проверки определяется для участников всех команд, которые являются неактивными гостевыми пользователями.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Кроме того, так как эта проверка применяется ко всем командам, настройте свойство **instanceEnumerationScope** , чтобы указать все команды. Динамические группы и группы, назначаемые ролем, не включаются в эту проверку.

Эта проверка не будет включать пользователей прямого подключения B2B в команды с общими каналами. Чтобы включить пользователей прямого подключения B2B в команды с общими каналами, см. пример 11. Просмотр всех пользователей, назначенных команде [, включая пользователей прямого подключения B2B](#example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) в команде с общими каналами.


---

### <a name="example-7-review-all-assignment-to-entitlement-management-access-packages"></a>Пример 7. Просмотр всех назначений для пакетов доступа управления правами

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

---

### <a name="example-8-review-all-service-principals-assigned-to-a-privileged-role"></a>Пример 8. Просмотр всех субъектов-служб, назначенных привилегированной роли

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-9-review-all-users-assigned-to-a-privileged-role"></a>Пример 9. Проверка всех пользователей, которым назначена привилегированная роль 

#### <a name="review-all-users-assigned-to-a-privileged-role-all-active-and-eligible-assignments-included"></a>Просмотрите всех пользователей, которым назначена привилегированная роль (все активные и допустимые назначения).

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleDefinitions/{role ID}",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-eligible-assignment-to-a-privileged-role"></a>Проверка всех пользователей с соответствующим назначением привилегированной роли

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleEligibilityScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-active-assignment-to-a-privileged-role"></a>Проверка всех пользователей с активным назначением привилегированной роли

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(assignmentType eq 'Assigned' and isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

---

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>Настройка области с помощью principalResourceMembershipsScope

**PrincipalResourceMembershipsScope** предоставляет свойства **principalScopes** и **resourceScopes** для поддержки более специализированных параметров конфигурации для области объекта **accessReviewScheduleDefinition**. Эти возможности включают проверку доступа для нескольких субъектов или групп субъектов к нескольким ресурсам.

### <a name="example-10-review-all-inactive-guest-users-assigned-to-all-groups"></a>Пример 10. Просмотр всех неактивных гостевых пользователей, назначенных всем группам

В следующем примере проверка определяется для прямых участников всех групп, которые являются неактивными гостевыми пользователями. Гостевые пользователи считаются неактивными, если период их бездействия — 30 дней с даты начала экземпляра проверки доступа.

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

### <a name="example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels"></a>Пример 11. Просмотр всех пользователей, назначенных команде, включая пользователей прямого подключения B2B в команде с общими каналами

В этом примере областью проверки доступа являются все пользователи, которые являются членами команды или назначены общему каналу в команде. К ним относятся внутренние пользователи, прямые и транзитивные пользователи, пользователи службы совместной работы B2B и пользователи прямого подключения B2B.

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups/{groupId}/transitiveMembers/microsoft.graph.user",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/teams/{groupId}/channels?$filter=(membershipType eq 'shared')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

Чтобы просмотреть пользователей и команды прямого подключения B2B в общих каналах, `/teams/{groupId}/channels?$filter=(membershipType eq 'shared')` необходимо указать шаблон запроса в **объекте resourceScopes**. Во *всех командах* , например в [примере 6](#review-all-inactive-guest-users-assigned-to-all-teams), не будут включены пользователи и команды прямого подключения B2B в общих каналах.

> [!NOTE]
> Проверка доступа пользователей и команд прямого подключения B2B поддерживается только в одноэтабных проверках доступа, а не в многоэтабных проверках доступа.

### <a name="example-12-review-all-guest-users-assigned-to-a-directory-role"></a>Пример 12. Проверка всех гостевых пользователей, которым назначена роль каталога

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

## <a name="next-steps"></a>Дальнейшие действия

+ [Назначение рецензентов определению проверки доступа](/graph/accessreviews-reviewers-concept)
+ [Ознакомьтесь с руководствами](/graph/accessreviews-overview), чтобы узнать, как использовать API проверки доступа для проверки доступа к Azure AD ресурсам.
+ [Создание проверки доступа](/azure/active-directory/governance/create-access-review)
