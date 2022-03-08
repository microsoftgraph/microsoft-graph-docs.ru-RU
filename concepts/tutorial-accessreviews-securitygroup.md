---
title: Руководство. Используйте API обзоров доступа для просмотра доступа к группам безопасности
description: Группы безопасности Azure AD можно использовать для управления доступом к ресурсам. Используйте API обзоров доступа, чтобы подтвердить, что все члены группы безопасности нуждаются в членстве, а также в расширении доступа к ресурсам, заверенным группе безопасности.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: ccb305df3cc5dbdf21d97ce1b87791a6729d5df8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337399"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a>Руководство. Используйте API обзоров доступа для просмотра доступа к группам безопасности

API для проверки доступа в Microsoft Graph позволяет организациям проверять и проверять доступ, который удостоверения (также называемые директорами *)* назначены ресурсам организации. Один из наиболее эффективных и эффективных методов управления привилегиями доступа для директоров к другим ресурсам — это группы безопасности Azure AD. Например, сотни пользователей могут быть назначены группе безопасности, а группе безопасности назначен доступ к папке. С помощью API отзывов о доступе организации могут периодически засвидетельстовку принципов, имеющих доступ к таким группам, а также другие ресурсы в организации.

Предположим, вы используете группы безопасности Azure AD для назначения удостоверений (также называемых директоров *) доступа* к ресурсам в организации. Периодически необходимо засвидетельствуть, что все члены группы безопасности нуждаются в членстве, а также о доступе к ресурсам, заверенным группе безопасности.

В этом руководстве вы можете использовать API проверки доступа для проверки доступа к группе безопасности в клиенте Azure AD. Вы можете использовать Graph explorer или Postman для проверки вызовов API API отзывов доступа, прежде чем автоматизировать их в сценарий или приложение. Эта тестовая среда экономит время, помогая правильно определять и проверять запросы без повторнойкомпилации приложения.

## <a name="prerequisites"></a>Необходимые компоненты

Для завершения этого руководства необходимы следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5.
+ Во входе [Graph explorer](https://developer.microsoft.com/graph/graph-explorer) в роли глобального администратора или администратора управления удостоверением Azure AD.
  + [Необязательный] Откройте новое **окно браузера инкогнито**, **анонимное** или **inPrivate** . Далее в этом учебнике вы вопишитесь.
+ Следующие делегированные разрешения: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.

Согласие на необходимые разрешения в Graph Explorer:
1. Выберите значок передач параметров справа от сведений учетной записи пользователя, а затем выберите **разрешения Select**.

    :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Graph Microsoft." border="true":::

2. Прокрутите список разрешений для этих разрешений:
   + AccessReview (3), развинь, а затем выберите **AccessReview.ReadWrite.All**.
   + Группа (2), развиньте и выберите **Group.ReadWrite.All**.
  
    Выберите **Согласие** и во всплывающее окно выберите Согласие от имени организации, а затем выберите **Accept**, чтобы принять согласие на разрешения.

   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на Graph разрешений Майкрософт." border="true":::
   
>[!NOTE]
>Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.
   
## <a name="step-1-create-test-users-in-your-tenant"></a>Шаг 1. Создание тестовых пользователей в клиенте

Создайте трех новых тестовых пользователей, каждый раз запуская запрос ниже трех раз, изменяя значения свойств **displayName**, **mailNickname** и **userPrincipalName** . Запись ID трех новых тестовых пользователей.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@Contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
    "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
    "displayName": "Adele Vance",
    "userPrincipalName": "AdeleV@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a>Шаг 2. Создание группы безопасности, назначение владельцев и добавление участников

Создайте группу безопасности с именем **Building security** , которая является целью обзоров доступа в этом руководстве. Назначьте этой группе одного владельца группы и двух участников.

### <a name="request"></a>Запрос

На предыдущем этапе вы создали три тестовых пользователя. Один из пользователей будет владельцем группы, а два других будут членами группы.

В этом вызове замените:
+ `d3bcdff4-4f80-4418-a65e-7bf3778c5dca` с ИД владельца группы.
+ `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` и `bf59c5ba-5304-4c9b-9192-e5a4cb8444e7` с ID-ами двух участников группы.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
    "description": "Building security",
    "displayName": "Building security",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/d3bcdff4-4f80-4418-a65e-7bf3778c5dca"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
        "https://graph.microsoft.com/beta/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7"
    ]
}
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
    "description": "Building security",
    "displayName": "Building security",
    "mailNickname": "buildingsecurity",
    "securityEnabled": true
}
```

В ответе зафиксировать ID новой группы, чтобы использовать его позже в этом руководстве.

## <a name="step-3-create-an-access-review-for-the-security-group"></a>Шаг 3. Создание обзора доступа для группы безопасности

### <a name="request"></a>Запрос

В этом вызове замените следующие значения:
+ `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` с ID группы **безопасности здания** . Область указывает, что проверка применяется к всем членам группы безопасности **здания** . Дополнительные параметры настройки области см. в разделе [See also](#see-also) .
+ Значение **startDate с** сегодняшней датой и значением **endDate** с датой пять дней с даты начала.

Обзор доступа имеет следующие параметры:

+ Это самообследование, как вывод, если вы не указываете значение для свойства **рецензентов** . Поэтому каждый член группы будет самостоятельно засвидетельстовывать необходимость сохранения доступа к группе.
+ Областью обзора являются члены (прямые и косвенные) группы **безопасности Здания** .
+ Рецензент должен предоставить обоснование необходимости поддерживать доступ к группе.
+ Решение по умолчанию принимается `Deny` в том случае, если рецензенты не отвечают на запрос на проверку доступа до истечения срока действия экземпляра. Решение `Deny` удаляет участников группы из группы.
+ Это разовая проверка доступа, которая заканчивается через пять дней. Поэтому после предоставления доступа пользователю не нужно повторно засвидетельстовка в течение периода проверки доступа.
+ Директора, которые определены в области обзора, будут получать уведомления и напоминания по электронной почте, побуждающие их самостоятельно подтвердить необходимость сохранения доступа.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "scope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
        "queryType": "MicrosoftGraph"
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
            }
        }
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
    "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
    "displayName": "One-time self-review for members of Building security",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "createdBy": {
        "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
        "displayName": "MOD Administrator",
        "type": null,
        "userPrincipalName": "admin@Contoso.com"
    },
    "scope": {},
    "instanceEnumerationScope": {},
    "reviewers": [],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

Состояние вышеуказанного обзора доступа помечено как **NotStarted**. Вы можете получить обзор доступа (GET `https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b`), чтобы отслеживать состояние, и когда он помечен как **InProgress**, тогда были созданы экземпляры для проверки доступа и решения могут быть размещены. Вы также можете получить обзор доступа, чтобы просмотреть полные параметры обзора доступа.

## <a name="step-4-list-instances-of-the-access-review"></a>Шаг 4. Список экземпляров обзора доступа

После того **как состояние** обзора доступа помечено `InProgress`как, запустите следующий запрос, чтобы перечислить все экземпляры определения обзора доступа. Так как в шаге 3 был создан разовая проверка доступа, запрос возвращает только один экземпляр с ИД, например, ИД определения расписания.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID определения обзора доступа, возвращенного в шаге 3.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances
```

### <a name="response"></a>Отклик

В этом ответе **состояние** `InProgress` экземпляра является тем, что **startDateTime** прошло, **а endDateTime** — в будущем. Если **startDateTime** будет в будущем, состояние будет .`NotStarted` С другой стороны, если **endDateTime** в прошлом, состояние будет `Completed`.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances",
    "value": [
        {
            "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "startDateTime": "2022-02-11T17:35:25.24Z",
            "endDateTime": "2022-02-16T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers/microsoft.graph.user",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [],
            "fallbackReviewers": []
        }
    ]
}
```

## <a name="step-5-who-was-contacted-for-the-review"></a>Шаг 5. Кто был связаться для проверки?

Вы можете подтвердить, что все члены группы безопасности **здания** связались для публикации решений по проверке для этого экземпляра обзора доступа.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID определения расписания проверки доступа.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_contactedReviewers"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/contactedReviewers
```

### <a name="response"></a>Отклик

В следующем ответе показано, что два члена группы безопасности **здания** были уведомлены об их ожидающих проверке.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewReviewer",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/contactedReviewers",
    "@odata.count": 2,
    "value": [
        {
            "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        },
        {
            "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "displayName": "Alex Wilber",
            "userPrincipalName": "AlexW@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        }
    ]
}
```

## <a name="step-6-get-decisions"></a>Шаг 6. Принятие решений

Вас интересуют решения, принятые в экземпляре обзора доступа.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID определения расписания просмотра доступа и экземпляра.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показаны решения, принятые в экземпляре обзора. Так **как безопасность здания** имеет два члена, ожидается два пункта решения.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4db68765-472d-4aa2-847a-433ea94bcfaf",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
                "displayName": "Alex Wilber",
                "type": "user",
                "userPrincipalName": "AlexW@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 5:31:37 PM +00:00"
            }
        },
        {
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 4:58:13 PM +00:00"
            }
        }
    ]
}
```

Из вызова свойство **решения** `NotReviewed` имеет значение, так как участники группы не завершили самоаттестацию. Следуйте шагу 7, чтобы узнать, как каждый член может самостоятельно подтвердить свою потребность в просмотре доступа.

## <a name="step-7-self-review-a-pending-access-decision"></a>Шаг 7. Самостоятельное рассмотрение ожидающих решения о доступе

На шаге 3 обзор доступа был настроен как самообсвечивающийся. Для этой конфигурации необходимо, чтобы оба члена группы безопасности **Здания** самостоятельно засвидетельяли необходимость сохранения доступа к группе.

>[!NOTE]
>Выполните этот шаг в качестве одного из двух членов группы безопасности **здания** .

На этом шаге вы перечислите ожидающих отзывов доступа, а затем завершите процесс самоаттестации. Этот шаг можно выполнить одним из двух способов, используя API или портал [My Access](https://myaccess.microsoft.com/). Другой рецензент не завершит этот процесс, и вместо этого вы позволите применять решения по умолчанию к их обзору доступа.

Запустите новый сеанс браузера **инкогнито****,** анонимного или **браузера InPrivate** и вопишитесь в качестве одного из двух членов группы безопасности **building**. Таким образом, вы не перебиваете текущий сеанс администратора. Мы впишемся в качестве Адель Вэнс. Кроме того, можно прервать текущий сеанс администратора, выйдя из Graph Explorer и войдя в систему в качестве одного из двух участников группы.

### <a name="method-1-use-the-access-reviews-api-to-self-review-pending-access"></a>Метод 1. Использование API обзоров доступа для самостоятельной проверки ожидающих доступа

#### <a name="list-your-access-reviews-decision-items"></a>Список элементов решений о просмотре доступа

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID определения расписания проверки доступа.

##### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/filterByCurrentUser(on='reviewer')
```

##### <a name="response"></a>Отклик
В ответе ниже вы (Адель Вэнс) имеете один ожидающих рассмотрения **доступа (**`NotReviewed`решение) для самостоятельной проверки. **Основные** свойства **и свойства ресурсов** указывают принцип, к которому применяется решение, и ресурс, к которому доступ находится на рассмотрении. В этом случае Adele Vance и **группа безопасности здания** соответственно.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/15/2022 9:35:23 AM +00:00"
            }
        }
    ]
}
```

#### <a name="record-a-decision"></a>Запись решения

Чтобы завершить обзор доступа, Адель Вэнс подтвердит необходимость сохранения доступа к **группе безопасности здания** .

##### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID `c7de8fba-4d6a-4fab-a659-62ff0c02643d` определения расписания проверки доступа и ID элемента ожидающих решений, возвращенного на предыдущем шаге.

```http
PATCH https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/c7de8fba-4d6a-4fab-a659-62ff0c02643d

{
    "decision": "Approve",
    "justification": "As the assistant security manager, I still need access to the building security group."
}
```

##### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
```


#### <a name="verify-the-decisions"></a>Проверка решений

Чтобы проверить решения, которые были записаны для проверки доступа, укай список элементов решений по [обзору доступа](#list-your-access-reviews-decision-items). Хотя период проверки доступа не истек, а решения не применяются, **applyResult** `New` будет помечен как и вы можете изменить решение.

Теперь можно выйти из сеанса браузера инкогнито и выйти из него.

### <a name="method-2-use-the-my-access-portal"></a>Метод 2. Использование портала "Мой доступ"

Рецензенты также могут посетить портал ["Мой доступ"](https://myaccess.microsoft.com/) , чтобы проверить ожидающих экземпляров проверки доступа.

+ Список ожидающих отзывов доступа. Пользователь может следовать одному из двух способов добраться туда:
  + Вариант 1. Выберите **кнопку доступа к** обзору из уведомления электронной почты, полученного в почтовом ящике. Уведомление электронной почты похоже на следующий снимок экрана. Выбор этой кнопки направляет их в ожидающийся обзор доступа.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/emailnotification.png" alt-text="Уведомление по электронной почте, чтобы просмотреть доступ." border="true":::

  + Вариант 2. Перейдите на [портал My Access](https://myaccess.microsoft.com/) . Выберите меню **Обзоры доступа** и выберите вкладку **Группы и Приложения** .

+ Из списка обзоров доступа выберите обзор доступа, для которого необходимо опубликовать решение. Выберите **Да** , чтобы опубликовать решение, которое по-прежнему необходимо для обеспечения **безопасности здания**. Введите причину, а затем выберите **Отправить**.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Самоопроверять необходимость сохранения доступа к ресурсу.":::


Теперь можно выйти из сеанса браузера инкогнито и выйти из него.

## <a name="step-8-confirm-the-decisions-and-the-status-of-the-access-review"></a>Шаг 8. Подтверждение решений и состояния обзора доступа

Возвращаясь к основному сеансу браузера, в котором вы все еще вошли в качестве глобального администратора, повторите шаг 4, чтобы увидеть, что свойство решения для Адель Вэнс теперь .`Approve` По истечении или истечении `Deny` срока действия проверки доступа решение по умолчанию будет записано для Алекса Уилбера. Затем решения будут автоматически применены, так как был задаток **autoApplyDecisionsEnabled** `true` и период экземпляра проверки доступа будет завершен. Затем Адель будет поддерживать доступ к группе безопасности **здания** , а Алекс автоматически будет удален из группы.

Поздравляем! Вы создали обзор доступа и самостоятельно засвидетельстировали необходимость поддержания доступа. Вы только один раз самостоятельно засвидетельстовывалось и `Deny` будете поддерживать доступ до тех пор, пока он не будет удален с помощью решения другого экземпляра проверки доступа или другого внутреннего процесса.

## <a name="step-9-clean-up-resources"></a>Шаг 9. Очистка ресурсов

Удалите ресурсы, созданные для этого руководства: группу безопасности здания, определение расписания просмотра доступа и трех тестовых пользователей.

### <a name="delete-the-security-group"></a>Удаление группы безопасности

#### <a name="request"></a>Запрос

В этом вызове замените `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` **id** безопасности **Building**.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-access-review-definition"></a>Удаление определения обзора доступа

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID определения обзора доступа. Так как определение расписания просмотра доступа является планом обзора доступа, удаление определения удаляет параметры, экземпляры и решения.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-three-test-users"></a>Удаление трех тестовых пользователей
В этом вызове замените `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` ID одного из тестовых пользователей. Повторите этот шаг дважды с помощью ID-данных двух других пользователей, чтобы удалить их.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>Заключение

Вы создали обзор доступа, в котором директора самостоятельно засвидетельировали необходимость сохранения доступа к ресурсу, в данном случае группе безопасности **building** .

В этом руководстве был продемонстрирован один из сценариев API обзоров доступа Azure AD. API обзоров доступа поддерживает различные сценарии с помощью сочетания ресурсов, директоров и рецензентов в соответствии с вашими потребностями в проверке доступа. Дополнительные сведения см. в [API отзывов о доступе](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true).

## <a name="see-also"></a>См. также

+ [API обзоров доступа](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true)
+ [Что такое обзоры доступа к Azure AD?](/azure/active-directory/governance/access-reviews-overview)
+ [Просмотрите доступ для себя к группам или приложениям в отзывах о доступе Azure AD](/azure/active-directory/governance/review-your-access)