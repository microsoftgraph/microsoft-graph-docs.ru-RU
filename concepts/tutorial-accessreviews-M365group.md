---
title: Руководство. Использование API проверок доступа для проверки гостевого доступа к группам Microsoft 365
description: Узнайте, как использовать API проверки доступа для проверки доступа внешних и гостевых пользователей к ресурсам организации через группы Microsoft 365 в Azure AD клиенте.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 972a3cb1aa8618370cf78d5921d16a699dd6b0b8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437564"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>Руководство. Использование API проверок доступа для проверки гостевого доступа к группам Microsoft 365

API проверок доступа в Microsoft Graph позволяет организациям выполнять аудит и аттестацию доступа, который удостоверения (также называемые субъектами *)* назначаются ресурсам в организации. При совместной работе между клиентами внешние пользователи могут получать доступ к таким ресурсам, как файлы, заметки, календари и даже беседы Teams. Этим доступом можно эффективно управлять с помощью групп Microsoft 365. Таким образом, с помощью API проверки доступа организации могут периодически выполнять аттестацию субъектов, которые имеют доступ к таким группам, а также по расширению других ресурсов в организации.

Предположим, что вы предоставили внешним пользователям (также называемым гостевыми пользователями) доступ к ресурсам в организации через группы Microsoft 365. В этом руководстве описано, как получить доступ к группам Microsoft 365 в клиенте.

>[!NOTE]
>Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости.

## <a name="prerequisites"></a>Предварительные требования

Для работы с этим руководством вам потребуются следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5. 
+ Учетная запись в другом клиенте Azure AD или удостоверении социальной сети, которую можно пригласить в качестве гостевого пользователя (B2B-пользователя).
+ Войдите в [песочницу Graph от](https://developer.microsoft.com/graph/graph-explorer) имени пользователя с ролью глобального администратора. 
+ Следующие делегированные разрешения: `User.Invite.All`, `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`, `User.ReadWrite.All`.

Чтобы дать согласие на необходимые разрешения в песочнице Graph, скажите следующее:
1. Щелкните значок параметров справа от сведений об учетной записи пользователя, а затем выберите " **Выбрать разрешения"**.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Microsoft Graph." border="true":::

2. Прокрутите список разрешений до следующих разрешений:
   + AccessReview (3), разверните и выберите **AccessReview.ReadWrite.All**.
   + Группу (2), разверните и выберите **Group.ReadWrite.All**.
   + Пользователь (8), разверните и выберите **User.Invite.All** и **User.ReadWrite.All**.
   
   Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно давать согласие от имени вашей организации на эти разрешения.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на разрешения Microsoft Graph." border="true":::

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

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>Шаг 2. Приглашение гостевого пользователя в клиент

Пригласите гостевого пользователя с адресом **электронной почты, john@tailspintoys.com** в клиент.

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

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>Шаг 3. Создание группы Microsoft 365 и добавление гостевого пользователя

На этом шаге:
1. Создайте новую группу Microsoft 365 с **именем Feel good marketing campaign**.
2. Назначьте себя владельцем группы.
3. Добавьте john@tailspintoys.com в качестве участника группы. Их доступ к группе является предметом проверки вами, владельцем группы.

### <a name="request"></a>Запрос

В этом вызове замените:
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` с идентификатором. Чтобы получить идентификатор, выполните команду `GET` `https://graph.microsoft.com/v1.0/me`.
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

Теперь у вас есть группа Microsoft 365 с гостевым пользователем.

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>Шаг 4. Создание проверки доступа для всех групп Microsoft 365 с гостевыми пользователями

При создании серии повторяющихся проверок доступа для всех групп Microsoft 365 с гостевыми пользователями вы запланируете периодическое просмотр доступа гостей к группе Microsoft 365. В этом случае группа **маркетинговой кампании Feel good** .

В серии проверки доступа используются следующие параметры:
+ Это повторяющаяся проверка доступа, которая просматривается ежеквартально.
+ Владельцы групп решают, следует ли гостевым пользователям поддерживать доступ.
+ Область проверки ограничена только группами Microsoft 365 с **гостевыми пользователями**.
+ Проверятель резервного копирования. Это может быть резервный пользователь или группа, которая может проверить доступ, если группе не назначены владельцы.
+ **Свойству autoApplyDecisionsEnabled** задано значение `true`. В этом случае решения применяются автоматически после завершения проверки доступа рецензентом или окончания срока проверки доступа. Если этот параметр не включен, пользователь должен применить решения вручную после завершения проверки.
+ **Примените действие removeAccessApplyAction** к запрещенным гостевым пользователям, чтобы удалить их из группы. Гостевой пользователь по-прежнему может войти в клиент, но не сможет получить доступ к группе.

### <a name="request"></a>Запрос

В этом вызове замените следующие значения:

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` с идентификатором Aline, которого вы назначаете в качестве рецензента резервного копирования.
+ Значение **startDate с** текущей датой и значением **endDate** с датой один год от даты начала. 

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

## <a name="step-5-list-instances-of-the-access-review"></a>Шаг 5. Перечисление экземпляров проверки доступа

В следующем запросе перечислены все экземпляры определения проверки доступа. Если в клиенте есть несколько групп Microsoft 365 с гостевыми пользователями, этот запрос вернет по одному экземпляру для каждой группы *Microsoft 365 с гостевыми пользователями*.

### <a name="request"></a>Запрос

В этом вызове замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` идентификатор определения проверки доступа, возвращенного на шаге 4.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>Отклик

В этом ответе область включает группу, `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` определенную группой (группа маркетинговой кампании **Feel good** , созданная на шаге 3), так как в ней есть гостевой пользователь.

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
В этом ответе в настоящее время используется экземпляр проверки доступа `InProgress`. Так как это ежеквартальное рассмотрение, новый экземпляр проверки создается автоматически каждые три месяца, и рецензенты могут применять новые решения.

## <a name="step-6-get-decisions"></a>Шаг 6. Получение решений

Получение решений, принятых для экземпляра проверки доступа.

### <a name="request"></a>Запрос

В этом вызове:
+ Замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` идентификатор определения проверки доступа, возвращенного на шаге 4.
+ Замените `6392b1a7-9c25-4844-83e5-34e23c88e16a` идентификатор экземпляра проверки доступа, возвращенного на шаге 5.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показано решение, принятое для экземпляра проверки.

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

В ежеквартальной проверке, такой как эта, и при условии, что проверка доступа по-прежнему активна:
+ Каждые три месяца создается новый экземпляр проверки.
+ Рецензентам потребуется применить новые решения для новых экземпляров.


## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Удалите ресурсы, созданные для этого руководства. Вы можете использовать хорошую группу маркетинговой кампании, определение расписания проверки доступа, гостевого пользователя и тестового пользователя.

### <a name="delete-the-microsoft-365-group"></a>Удаление группы Microsoft 365

#### <a name="request"></a>Запрос

В этом вызове замените `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` идентификатор вашей маркетинговой кампании **Feel good** группой Microsoft 365.

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

### <a name="delete-the-access-review-definition"></a>Удаление определения проверки доступа

В этом вызове замените `c22ae540-b89a-4d24-bac0-4ef35e6591ea` идентификатор определения проверки доступа. Так как определение расписания проверки доступа является схемой для проверки доступа, удаление определения приведет к удалению связанных параметров, экземпляров и решений.

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

В этом вызове замените `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` идентификатор гостевого пользователя, john@tailspintoys.com.

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
В этом вызове замените `c9a5aff7-9298-4d71-adab-0a222e0a05e4` идентификатор тестового пользователя.

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

Поздравляем! Вы создали проверку доступа для гостевых пользователей в группах Microsoft 365 в клиенте и запланируете ее ежеквартально. Владельцы групп будут проверять доступ в течение этих циклов, выбирая утверждение или запрет доступа.

## <a name="see-also"></a>См. также


+ [API проверки доступа](/graph/api/resources/accessreviewsv2-overview)
+ [Что такое Azure AD доступа?](/azure/active-directory/governance/access-reviews-overview)
+ [Проверка доступа к группам и приложениям в Azure AD проверки доступа](/azure/active-directory/governance/perform-access-review)