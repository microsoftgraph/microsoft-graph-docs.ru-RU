---
title: Руководство. Используйте API обзоров доступа для просмотра гостевого доступа к группам Microsoft 365.
description: Используйте API отзывов доступа, чтобы просмотреть гостевой доступ к группам Microsoft 365.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: f2c9210b4173850c6fbccaad352c88b894965e29
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334921"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>Руководство. Используйте API обзоров доступа для просмотра гостевого доступа к группам Microsoft 365.

API для проверки доступа в Microsoft Graph позволяет организациям проверять и проверять доступ, который удостоверения (также называемые директорами *)* назначены ресурсам организации. В совместной работе с клиентом внешние пользователи могут получать доступ к ресурсам, таким как файлы, заметки, календари и даже Teams беседы. Этот доступ можно эффективно управлять Microsoft 365 группами. Таким образом, с помощью API отзывов о доступе организации могут периодически засвидетельстовки принципов, имеющих доступ к таким группам, а также других ресурсов организации.

Предположим, что вы предоставили доступ внешним пользователям (также называемым гостевых *) к* ресурсам в вашей организации Microsoft 365 группами. В этом руководстве вы сможете просмотреть их доступ к группам Microsoft 365 в клиенте.

>[!NOTE]
>Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.

## <a name="prerequisites"></a>Предварительные условия

Для завершения этого руководства необходимы следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5. 
+ Учетная запись в другом клиенте Azure AD или социальном удостоверении, которую можно пригласить в качестве гостевого пользователя (B2B-пользователя).
+ Вопишите Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя в роли глобального администратора. 
+ Следующие делегированные разрешения: `User.Invite.All`, , `Group.ReadWrite.All``AccessReview.ReadWrite.All``User.ReadWrite.All`.

Согласие на необходимые разрешения в Graph Explorer:
1. Выберите значок параметров справа от сведений учетной записи пользователя, а затем Выберите **разрешения**.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Graph Microsoft." border="true":::

2. Прокрутите список разрешений для этих разрешений:
   + AccessReview (3), развинь, а затем выберите **AccessReview.ReadWrite.All**.
   + Группа (2), развиньте и выберите **Group.ReadWrite.All**.
   + Пользователь (8), расширить и затем выбрать **User.Invite.All** и **User.ReadWrite.All**.
   
   Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно соглашаться от имени организации на эти разрешения.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на Graph разрешений Майкрософт." border="true":::

## <a name="step-1-create-a-test-user-in-your-tenant"></a>Шаг 1. Создание тестового пользователя в клиенте

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-createUser"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>Шаг 2. Приглашение гостевого пользователя в клиента

Приглашение гостевого пользователя с адресом **электронной почты john@tailspintoys.com** клиенту.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-inviteguest"
}-->

```http
POST https://graph.microsoft.com/v1.0/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>Шаг 3. Создание Microsoft 365 группы и добавление гостевого пользователя

На этом шаге:
1. Создайте новую Microsoft 365 с именем **Feel good marketing campaign**.
2. Назначьте себя владельцем группы.
3. Добавьте john@tailspintoys.com в качестве участника группы. Их доступ к группе является предметом рассмотрения вами, владельцем группы.

### <a name="request"></a>Запрос

В этом вызове замените:
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` с вашим ИД. Чтобы получить свой ID, запустите `GET` .`https://graph.microsoft.com/v1.0/me`
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` с **john@tailspintoys.com** из ответа на шаге 2.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
    "description": "Feelgood Marketing Campaign with external partners and vendors.",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ],
    "mailEnabled": true,
    "mailNickname": "FeelGoodCampaign",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

Теперь у вас Microsoft 365 группа с гостевых пользователей.

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>Шаг 4. Создание обзора доступа для всех групп Microsoft 365 с гостевых пользователей

При создании серии повторных обзоров доступа для всех групп Microsoft 365 с гостевых пользователей вы запланировать периодический обзор доступа гостей к Microsoft 365 группе. В этом случае группа **Маркетинговой кампании Feel good** .

В серии обзоров доступа используются следующие параметры:
+ Это повторяющийся обзор доступа, который пересматривается ежеквартно.
+ Владельцы групп решают, следует ли гостевых пользователей поддерживать свой доступ.
+ Область обзора ограничивается только группами Microsoft 365 с **гостевых пользователей**.
+ Обозреватель резервного копирования. Они могут быть пользователем-откатом или группой, которая может просмотреть доступ в случае, если у группы нет владельцев.
+ **autoApplyDecisionsEnabled** установлено для `true`. В этом случае решения применяются автоматически, как только рецензент завершит обзор доступа или закончится продолжительность обзора доступа. Если он не включен, пользователь должен применять решения вручную после завершения проверки.
+ Применить действие **removeAccessApplyAction** к отклоненным гостевых пользователям, чтобы удалить их из группы. Гостевой пользователь по-прежнему может войти в клиент, но не будет получать доступ к группе.

### <a name="request"></a>Запрос

В этом вызове замените следующие значения:

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` с ИД Aline, который вы назначаете в качестве резервного рецензента.
+ Значение **startDate с** сегодняшней датой и **значением endDate** с датой один год с даты начала. 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "c22ae540-b89a-4d24-bac0-4ef35e6591ea",
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "status": "NotStarted",
    "createdBy": {
        "id": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-5-list-instances-of-the-access-review"></a>Шаг 5. Список экземпляров обзора доступа

В следующем запросе перечислены все экземпляры определения обзора доступа. Если в клиенте Microsoft 365 несколько групп с гостевых пользователей, этот запрос возвращает по одному экземпляру для каждой Microsoft 365 с *гостевых пользователей*.

### <a name="request"></a>Запрос

В этом вызове замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` ID определения обзора доступа, возвращенного в шаге 4.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>Отклик

В этом ответе `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` область включает группу, идентифицированную группой (группа маркетинговой кампании **Feel good** , созданная в шаге 3), так как у нее есть гостевой пользователь.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
    "value": [
        {
            "id": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "startDateTime": "2021-02-10T17:00:36.96Z",
            "endDateTime": "2021-02-10T17:00:36.96Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
В этом ответе экземпляр проверки доступа в настоящее время `InProgress`. Поскольку это ежеквартный обзор, новый экземпляр обзора создается автоматически каждые три месяца, и рецензенты могут применять новые решения.

## <a name="step-6-get-decisions"></a>Шаг 6. Принятие решений

Получите решения, принятые в случае проверки доступа.

### <a name="request"></a>Запрос

В этом вызове:
+ Замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` ID определения обзора доступа, возвращенного в шаге 4.
+ Замените `6392b1a7-9c25-4844-83e5-34e23c88e16a` ID экземпляра обзора доступа, возвращенного в шаге 5.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показано решение, принятое для экземпляра обзора.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "0e76ee07-b4c6-469e-bc9d-e73fc9a8d660",
            "accessReviewId": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "reviewedDateTime": "2021-02-10T17:06:26.147Z",
            "decision": "Approve",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "AAD Access Reviews",
                "userPrincipalName": "AAD Access Reviews"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "userDisplayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "displayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            }
        }
    ]
}
```

В ежеквартовом обзоре, как этот, и до тех пор, как обзор доступа по-прежнему активен:
+ Каждые три месяца будет создаваться новый экземпляр обзора.
+ Рецензенты должны будут применять новые решения для новых экземпляров.


## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Удалите ресурсы, созданные для этого учебного **руководства. Вы** можете использовать группу маркетинговой кампании, определение расписания просмотра доступа, гостевой пользователь и тестовый пользователь.

### <a name="delete-the-microsoft-365-group"></a>Удаление Microsoft 365 группы

#### <a name="request"></a>Запрос

В этом вызове замените `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` ID вашей маркетинговой кампании **Feel good Microsoft 365** группы.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a>Удаление определения обзора доступа

В этом вызове замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` ID определения обзора доступа. Так как определение расписания проверки доступа является планом обзора доступа, удаление определения удаляет связанные параметры, экземпляры и решения.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="remove-the-guest-user"></a>Удаление гостевого пользователя

В этом вызове замените `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` ID гостевого пользователя john@tailspintoys.com.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a>Удаление тестового пользователя
В этом вызове замените `c9a5aff7-9298-4d71-adab-0a222e0a05e4` ID тестового пользователя.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_guestuser"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

Поздравляем! Вы создали обзор доступа для гостевых пользователей в Microsoft 365 в клиенте и запланнесли его ежеквартно. Владельцы групп будут пересматривать доступ во время этих циклов, выбирая утверждение или отказ в доступе.

## <a name="see-also"></a>Дополнительные ресурсы


+ [API обзоров доступа](/graph/api/resources/accessreviewsv2-overview)
+ [Что такое обзоры доступа к Azure AD?](/azure/active-directory/governance/access-reviews-overview)
+ [Просмотр доступа к группам и приложениям в отзывах о доступе к Azure AD](/azure/active-directory/governance/perform-access-review)