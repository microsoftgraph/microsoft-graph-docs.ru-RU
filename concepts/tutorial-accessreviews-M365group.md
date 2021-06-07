---
title: Руководство. Используйте API обзоров доступа, чтобы просмотреть гостевой доступ к группам Microsoft 365.
description: Используйте API обзоров доступа, чтобы просмотреть гостевой доступ к группам Microsoft 365.
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: ad34932926a658d498242dd168ac7fee1d2b31a1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751141"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>Руководство. Используйте API обзоров доступа, чтобы просмотреть гостевой доступ к группам Microsoft 365.

В этом руководстве Graph Explorer для создания и чтения отзывов доступа, которые ориентированы на все Microsoft 365 группы с гостевых пользователей в клиенте. Для этого сначала с помощью Azure AD B2B вы сможете приглашать и создавать гостевого пользователя, также именуемого внешним удостоверением, в клиенте. Затем перед созданием и чтением обзора доступа вы добавите этого гостевых пользователей в Microsoft 365 группу.

>[!NOTE]
>Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.

## <a name="prerequisites"></a>Предварительные требования

Для завершения этого руководства необходимы следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной лицензией Azure AD Premium P2 или EMS E5. 
+ Учетная запись в другом клиенте Azure AD или социальном удостоверении, которую можно пригласить в качестве гостевого пользователя (B2B-пользователя).
+ Вопишитесь [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя в роли глобального администратора. 
+ Следующие делегированные разрешения: `User.Invite.All` `AccessReview.ReadWrite.All` , , `Group.ReadWrite.All` `User.ReadWrite.All` .

Согласие на необходимые разрешения в Graph Explorer:
1. Выберите значок параметров справа от сведений учетной записи пользователя, а затем выберите **Выберите разрешения.**
   
   ![Выбор разрешений Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. Прокрутите список разрешений для этих разрешений:
   + AccessReviews (3), расширяйте и выберите **AccessReviews.ReadWrite.All**.
   + Группа (2), развиньте и выберите **Group.ReadWrite.All**.
   + Пользователь (8), расширить и затем выбрать **User.Invite.All** и **User.ReadWrite.All**.
   
   Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно предоставлять согласие от имени организации для этих разрешений.
   
   ![Согласие на разрешения Graph Майкрософт](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-a-test-user-in-your-tenant"></a>Шаг 1. Создание тестового пользователя в клиенте

### <a name="request"></a>Запрос

```http
POST /users
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

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>Шаг 2. Приглашение гостевого пользователя в клиента

Приглашение гостевого пользователя с адресом **электронной почты john@tailspintoys.com** клиенту.

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a>Отклик

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>Шаг 3. Создание Microsoft 365 группы и добавление гостевого пользователя

На этом шаге:
1. Создайте новую Microsoft 365 с именем **маркетинговая кампания Feelgood.**
2. Назначьте себя владельцем группы.
3. Добавьте john@tailspintoys.com в качестве участника группы. Их доступ к группе является предметом рассмотрения вами, владельцем группы.

### <a name="request"></a>Запрос
В этом вызове замените:
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` с **вашим id**. Чтобы получить свой **id,** `GET` запустите `https://graph.microsoft.com/beta/me` .
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` с **john@tailspintoys.com**'s **id** из ответа в шаге 2.

```http
POST https://graph.microsoft.com/beta/groups
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
        "https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a>Отклик

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

Теперь у вас Microsoft 365 группа с гостевых пользователей.

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>Шаг 4. Создание обзора доступа для всех групп Microsoft 365 с гостевых пользователей

При создании серии повторяющихся обзоров доступа для всех групп Microsoft 365 с гостевых пользователей вы запланировать периодический обзор доступа гостей к группе Microsoft 365. Сделайте это для **группы маркетинговой кампании Feelgood.**

В серии обзоров доступа используются следующие параметры:
+ Это повторяющийся обзор доступа, который пересматривается ежеквартно.
+ Владельцы групп проверяют постоянный доступ гостевых пользователей.
+ Область обзора ограничивается только Microsoft 365 только с **гостевых пользователей.** Дополнительные параметры настройки области см. в разделе [See also.](#see-also) 
+ Обозреватель резервного копирования. Это может быть пользователь с откатом или группа, которая может просмотреть доступ в случае, если у группы нет владельцев. Дополнительные возможности настройки рецензентов см. в разделе [See also.](#see-also)
+ **autoApplyDecisionsEnabled** установлено `true` для . В этом случае решения применяются автоматически, как только рецензент завершит обзор доступа или закончится продолжительность обзора доступа. Если он не включен, пользователь должен после завершения проверки применять решения вручную.
+ Применить **действие removeAccessApplyAction** для отклонить гостевых пользователей. Это удаляет членство в группе отклоненного гостя. Гостевой пользователь по-прежнему может войти в клиент.

### <a name="request"></a>Запрос
В этом вызове замените следующее:

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` с **ид пользователя,** назначенного в качестве резервного рецензента. Это **id из** ответа в шаге 1.
+ Значение **startDate с** сегодняшней датой и **значением endDate** с датой один год с даты начала. 

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
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
    "backupReviewers": [
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

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
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
    "backupReviewers": [
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

В следующем запросе перечислены все экземпляры определения обзора доступа. Если клиент тестирования содержит другие группы Microsoft 365 с гостевых пользователей, этот запрос возвращает один экземпляр для каждой Microsoft 365 группы с гостевых пользователей в клиенте.

### <a name="request"></a>Запрос
В этом вызове `c22ae540-b89a-4d24-bac0-4ef35e6591ea` замените **id** определения обзора доступа, возвращенного в шаге 4.

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>Отклик
В этом ответе область включает группу с **id** (группа маркетинговой кампании `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **Feelgood,** созданная в шаге 3), так как у нее есть гость.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
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
В этом ответе экземпляр проверки доступа в настоящее время `InProgress` . Поскольку это ежеквартный обзор, каждые 3 месяца новый экземпляр обзора создается автоматически, и вы — рецензент — можете применять новые решения.

## <a name="step-6-get-decisions"></a>Шаг 6. Принятие решений

Получите решения, принятые в случае проверки доступа.

### <a name="request"></a>Запрос
В этом вызове:
+ `c22ae540-b89a-4d24-bac0-4ef35e6591ea`Замените **id определения** обзора доступа, возвращенного в шаге 4.
+ `6392b1a7-9c25-4844-83e5-34e23c88e16a`Замените **id экземпляра** обзора доступа, возвращенного в шаге 5.

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показано решение, принятое для экземпляра обзора.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
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

Так как это ежекварточный обзор, и пока определение по-прежнему активно, то есть периодичная дата повторения не является прошлой датой, каждые 3 месяца, когда создается новый экземпляр обзора, вы, как рецензент, можете применять новые решения. 

## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Удалите ресурсы, созданные для этого руководства: группу маркетинговой кампании **Feelgood,** определение расписания обзоров доступа, гостевой пользователь и тестовый пользователь.

### <a name="delete-the-microsoft-365-group"></a>Удаление Microsoft 365 группы

#### <a name="request"></a>Запрос
В этом вызове замените id маркетинговой кампании `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **Feelgood** Microsoft 365 группы. 

```http
DELETE https://graph.microsoft.com/beta/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a>Удаление определения обзора доступа

В этом вызове `c22ae540-b89a-4d24-bac0-4ef35e6591ea` замените **id** определения обзора доступа. Так как определение расписания проверки доступа является планом обзора доступа, удаление определения удаляет параметры, экземпляры и решения, связанные с обзором доступа.

#### <a name="request"></a>Запрос
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a>Отклик
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```
### <a name="remove-the-guest-user"></a>Удаление гостевого пользователя

В этом вызове `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` замените **id** гостевого пользователя john@tailspintoys.com.

#### <a name="request"></a>Запрос
```http
DELETE https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a>Отклик
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a>Удаление тестового пользователя

#### <a name="request"></a>Запрос
В этом вызове `c9a5aff7-9298-4d71-adab-0a222e0a05e4` замените **id** тестового пользователя.

```http
DELETE https://graph.microsoft.com/beta/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

Поздравляем! Вы создали обзор доступа для всех гостевых пользователей в Microsoft 365 группах в клиенте и запланирование ежеквартов для оценки и аттестации доступа гостевых пользователей. Владельцы групп будут пересматривать доступ во время этих циклов, выбирая утверждение или отказ в доступе.

## <a name="see-also"></a>См. также

+ [Ссылка на API обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [Настройка области определения обзора доступа с помощью API microsoft Graph](/graph/accessreviews-scope-concept)
+ [Назначение рецензентов определению обзора доступа с помощью API Graph Microsoft](/graph/accessreviews-reviewers-concept)
+ [Обзор обзоров доступа и требования к лицензиям](/azure/active-directory/governance/access-reviews-overview)
+ [Создание обзора доступа групп & приложений](/azure/active-directory/governance/create-access-review)
+ [Приглашение и добавление гостевых пользователей в организацию](/graph/api/resources/invitation?view=graph-rest-beta&preserve-view=true)

