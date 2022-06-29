---
title: Руководство. Использование API проверок доступа для проверки доступа к группам безопасности
description: Узнайте, как использовать API проверок доступа для проверки доступа к группе безопасности в клиенте Azure AD и тестирования вызовов API перед их автоматизацией в скрипты или приложения.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 7f64afebad0057b305aa5c3dc2544753aad8d25f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443811"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a>Руководство. Использование API проверок доступа для проверки доступа к группам безопасности

API проверок доступа в Microsoft Graph позволяет организациям выполнять аудит и аттестацию доступа, который удостоверения (также называемые субъектами *)* назначаются ресурсам в организации. Одним из наиболее эффективных и эффективных методов управления привилегиями доступа для субъектов к другим ресурсам является использование Azure AD безопасности. Например, сотни пользователей могут быть назначены группе безопасности, а группе безопасности — доступ к папке. С помощью API проверки доступа организации могут периодически проверять участников, которые имеют доступ к таким группам, а также по расширению других ресурсов в организации.

Предположим, вы используете Azure AD безопасности для назначения удостоверениям (также называемым *субъектами) доступа* к ресурсам в организации. Периодически необходимо подтвердить, что все члены группы безопасности должны быть участниками и по расширению доступа к ресурсам, назначенным группе безопасности.

В этом руководстве показано, как использовать API проверок доступа для проверки доступа к группе безопасности в Azure AD клиенте. Вы можете использовать песочницу Graph или Postman для тестирования вызовов API проверок доступа, прежде чем автоматизировать их в сценарий или приложение. Эта тестовая среда экономит время, помогая правильно определять и проверять запросы без повторной компиляции приложения.

## <a name="prerequisites"></a>Предварительные требования

Для работы с этим руководством вам потребуются следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5.
+ Войдите в [песочницу Graph от](https://developer.microsoft.com/graph/graph-explorer) имени пользователя с ролью глобального администратора или администратора Azure AD удостоверений.
  + [Необязательно] Откройте новое окно **браузера inognito**, **anonymous** или **InPrivate** . Вы выполните вход позже в этом руководстве.
+ Следующие делегированные разрешения: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.

Чтобы дать согласие на необходимые разрешения в песочнице Graph, скажите следующее:
1. Щелкните значок шестеренки параметров справа от сведений об учетной записи пользователя, а затем выберите " **Выбрать разрешения"**.

    :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Microsoft Graph." border="true":::

2. Прокрутите список разрешений до следующих разрешений:
   + AccessReview (3), разверните и выберите **AccessReview.ReadWrite.All**.
   + Группу (2), разверните и выберите **Group.ReadWrite.All**.
  
    Выберите **"Согласие**" и во всплывающем окне выберите "Согласие от имени организации", а затем выберите "Принять", чтобы принять согласие на разрешения.

   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на разрешения Microsoft Graph." border="true":::
   
>[!NOTE]
>Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости.
   
## <a name="step-1-create-test-users-in-your-tenant"></a>Шаг 1. Создание тестовых пользователей в клиенте

Создайте трех тестовых пользователей, выполнив приведенный ниже запрос три раза, изменив значения свойств **displayName**, **mailNickname** и **userPrincipalName** каждый раз. Запишите идентификаторы трех новых тестовых пользователей.

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

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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

Создайте группу безопасности с **именем Building security** , которая является целью проверок доступа в этом руководстве. Назначьте этой группе одного владельца группы и двух участников.

### <a name="request"></a>Запрос

На предыдущем шаге вы создали трех тестовых пользователей. Один из пользователей будет владельцем группы, а два других — участниками группы.

В этом вызове замените:
+ `d3bcdff4-4f80-4418-a65e-7bf3778c5dca` с идентификатором владельца группы.
+ `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` и `bf59c5ba-5304-4c9b-9192-e5a4cb8444e7` с идентификаторами двух участников группы.

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

В ответе запишите идентификатор новой группы, чтобы использовать его далее в этом руководстве.

## <a name="step-3-create-an-access-review-for-the-security-group"></a>Шаг 3. Создание проверки доступа для группы безопасности

### <a name="request"></a>Запрос

В этом вызове замените следующие значения:
+ `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` с идентификатором группы безопасности **Building** . Область указывает, что проверка применяется ко всем членам группы **безопасности Building** . Дополнительные параметры настройки области см. в разделе ["См. также](#see-also) ".
+ Значение **startDate с** текущей датой и **значением endDate** с датой в пять дней от даты начала.

Проверка доступа имеет следующие параметры:

+ Это самообслуживка, выводимая, если не указать значение для **свойства рецензентов** . Таким образом, каждый член группы самостоятельно подтверждает свою необходимость в обслуживании доступа к группе.
+ Областью проверки являются члены (прямые и косвенные) группы **безопасности "Построение** ".
+ Рецензент должен предоставить обоснование, почему ему необходимо поддерживать доступ к группе.
+ Решение по умолчанию принимается `Deny` , когда рецензенты не отвечают на запрос на проверку доступа до истечения срока действия экземпляра. Решение `Deny` удаляет участников группы из группы.
+ Это разовая проверка доступа, которая заканчивается через пять дней. Таким образом, после предоставления доступа пользователю не нужно повторно самостоять в течение периода проверки доступа.
+ Субъекты, определенные в области проверки, будут получать уведомления по электронной почте и напоминания с предложением самостоятельно подтвердить необходимость поддержки доступа.

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

Состояние вышеуказанной проверки доступа помечается как **NotStarted**. Вы можете получить проверку доступа (GET `https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b`) для отслеживания состояния и, если она помечена как **InProgress**, экземпляры были созданы для проверки доступа и могут публиковаться решения. Вы также можете получить проверку доступа, чтобы просмотреть полные параметры проверки доступа.

## <a name="step-4-list-instances-of-the-access-review"></a>Шаг 4. Перечисление экземпляров проверки доступа

После **пометки** состояния проверки доступа `InProgress`выполните следующий запрос, чтобы получить список всех экземпляров определения проверки доступа. Так как вы создали разовую проверку доступа на шаге 3, запрос возвращает только один экземпляр с идентификатором, таким как идентификатор определения расписания.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` идентификатор определения проверки доступа, возвращенного на шаге 3.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances
```

### <a name="response"></a>Отклик

В этом ответе состояние **экземпляра** `InProgress` связано с тем, что **startDateTime** находится в прошлом, **а endDateTime** — в будущем. Если **startDateTime** находится в будущем, состояние будет равно .`NotStarted` С другой стороны, если **endDateTime** находится в прошлом, состояние будет иметь значение .`Completed`

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

## <a name="step-5-who-was-contacted-for-the-review"></a>Шаг 5. С кем связывались для проверки?

Вы можете убедиться, что все члены  группы безопасности "Сборка" были зарегистрированы для публикации решений о проверке для этого экземпляра проверки доступа.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` идентификатор определения расписания проверки доступа.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_contactedReviewers"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/contactedReviewers
```

### <a name="response"></a>Отклик

В следующем ответе показано, что два члена группы безопасности " **Построение" были** уведомлены об ожидающей проверке.

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

## <a name="step-6-get-decisions"></a>Шаг 6. Получение решений

Вас интересуют решения, принятые для экземпляра проверки доступа.

### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` идентификатор определения расписания проверки доступа и экземпляра.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показаны решения, принятые в экземпляре проверки. Так **как безопасность при** построении включает два элемента, ожидается два элемента принятия решений.

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

В вызове свойство **принятия** решений `NotReviewed` имеет значение, так как участники группы еще не завершили самотестацию. Выполните шаг 7, чтобы узнать, как каждый участник может самостоятельно подтвердить свою необходимость в проверке доступа.

## <a name="step-7-self-review-a-pending-access-decision"></a>Шаг 7. Самостоятельное рассмотрение ожидающего решения о доступе

На шаге 3 проверка доступа настроена как самообслуживка. Для этой конфигурации необходимо, чтобы оба члена группы безопасности **"** Построение" самодоверялили свою необходимость в обслуживании доступа к группе.

>[!NOTE]
>Выполните этот шаг как один из двух членов группы **безопасности "Построение** ".

На этом шаге вы перечислите ожидающие проверки доступа, а затем завершите процесс самостоятельной аттестации. Этот шаг можно выполнить одним из двух способов: с помощью API или [портала "Мой доступ"](https://myaccess.microsoft.com/). Другой рецензент не завершит этот процесс, и вместо этого вы разрешите применять решения по умолчанию к проверке доступа.

Запустите новый **сеанс браузера в режиме инкогнито****,** анонимного или **InPrivate** и войдите в систему как один из двух членов группы **безопасности Building**. Это не приведет к прерыванию текущего сеанса администратора. Мы войдите как Адель Вэнс(Adele Vance). Кроме того, можно прервать текущий сеанс администратора, выполнив выход из песочнице Graph и выполнив вход в качестве одного из двух участников группы.

### <a name="method-1-use-the-access-reviews-api-to-self-review-pending-access"></a>Метод 1. Использование API проверок доступа для самостоятельной проверки ожидающего доступа

#### <a name="list-your-access-reviews-decision-items"></a>Вывод списка элементов принятия решений о проверке доступа

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` идентификатор определения расписания проверки доступа.

##### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/filterByCurrentUser(on='reviewer')
```

##### <a name="response"></a>Отклик
В приведенном ниже ответе (Adele Vance) у вас есть одна ожидающая проверка **доступа (**`NotReviewed`решение принимается) для самостоятельного подтверждения. Свойства **субъекта** **и** ресурса указывают субъект, к которому применяется решение, и ресурс, к которому выполняется проверка доступа. В этом случае Адель Вэнс (Adele Vance) и группа **безопасности Building (Сборка)** соответственно.

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

Чтобы завершить проверку доступа, Адель Вэнс подтвердит необходимость в обслуживании доступа к группе **безопасности "Построение** ".

##### <a name="request"></a>Запрос

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` `c7de8fba-4d6a-4fab-a659-62ff0c02643d` идентификатор определения расписания проверки доступа и идентификатор ожидающего элемента принятия решения, возвращенного на предыдущем шаге.

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

Чтобы проверить решения, которые вы записали для проверки доступа, [перечислите элементы принятия решений о проверке доступа](#list-your-access-reviews-decision-items). Хотя срок проверки доступа не истек, и решения не применяются, **applyResult** `New` будет помечен как и вы можете изменить решение.

Теперь вы можете выйти из сеанса браузера инкогнито и выйти из него.

### <a name="method-2-use-the-my-access-portal"></a>Метод 2. Использование портала "Мой доступ"

Рецензенты также могут посетить портал ["Мой доступ](https://myaccess.microsoft.com/) ", чтобы проверить ожидающие проверки экземпляры.

+ Вывод списка ожидающих проверок доступа. Пользователь может выполнить один из двух способов:
  + Вариант 1. Нажмите **кнопку "Проверить доступ** " в уведомлении по электронной почте, полученном в почтовом ящике. Уведомление по электронной почте похоже на следующий снимок экрана. Нажатие этой кнопки направляет их к ожидающей проверке доступа.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/emailnotification.png" alt-text="Уведомление по электронной почте для проверки доступа." border="true":::

  + Вариант 2. Перейдите на портал [портала "Мой доступ](https://myaccess.microsoft.com/) ". Выберите меню **"Проверки доступа** " и перейдите на вкладку **"Группы и приложения** ".

+ В списке проверок доступа выберите проверку доступа, для которой нужно опубликовать решение. Выберите **"Да** ", чтобы опубликовать решение о том, что вам по-прежнему нужен доступ к **службе "Безопасность здания"**. Введите причину и нажмите кнопку " **Отправить"**.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Самодостоять необходимость поддерживать доступ к ресурсу.":::


Теперь вы можете выйти из сеанса браузера инкогнито и выйти из него.

## <a name="step-8-confirm-the-decisions-and-the-status-of-the-access-review"></a>Шаг 8. Подтверждение решений и состояния проверки доступа

Вернитесь в основной сеанс браузера, где вы по-прежнему вошли в систему от имени глобального администратора, повторите шаг 4, чтобы увидеть, что свойство принятия решений для Adele Vance теперь имеет значение `Approve`. По завершении или истечении `Deny` срока действия проверки доступа для Алекса Вилбера будет записано решение по умолчанию. Затем решения будут автоматически применены, так как для **autoApplyDecisionsEnabled** `true` задано значение и срок действия экземпляра проверки доступа будет завершен. Затем Адель сохранит доступ к группе безопасности **"** Построение", а Алексей будет автоматически удален из группы.

Поздравляем! Вы создали проверку доступа и самостоятельно выполнили свою необходимость в обслуживании доступа. Вы только один раз `Deny` проходите самостояние и сохраняете доступ, пока он не будет удален с помощью решения другого экземпляра проверки доступа или другого внутреннего процесса.

## <a name="step-9-clean-up-resources"></a>Шаг 9. Очистка ресурсов

Удалите ресурсы, созданные для этого руководства: группу безопасности "Сборка", определение расписания проверки доступа и трех тестовых пользователей.

### <a name="delete-the-security-group"></a>Удаление группы безопасности

#### <a name="request"></a>Запрос

В этом вызове замените `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` **идентификатором** системы безопасности **building**.

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

### <a name="delete-the-access-review-definition"></a>Удаление определения проверки доступа

В этом вызове замените `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` идентификатор определения проверки доступа. Так как определение расписания проверки доступа является схемой для проверки доступа, удаление определения приведет к удалению параметров, экземпляров и решений.

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
В этом вызове замените `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` идентификатор одного из тестовых пользователей. Повторите этот шаг дважды с идентификаторами двух других пользователей, чтобы удалить их.

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

Вы создали проверку доступа, в которой участники самостоятельно выполнили свою необходимость в обслуживании доступа к ресурсу, в данном случае группе безопасности **"** Построение".

В этом руководстве демонстрируется один из сценариев API проверки Azure AD доступа. API проверок доступа поддерживает различные сценарии с помощью сочетания ресурсов, субъектов и рецензентов в соответствии с потребностями аттестации доступа. Дополнительные сведения см. в [API проверок доступа](/graph/api/resources/accessreviewsv2-overview).

## <a name="see-also"></a>См. также

+ [Что такое Azure AD доступа?](/azure/active-directory/governance/access-reviews-overview)
+ [Проверка доступа для себя к группам или приложениям в Azure AD проверки доступа](/azure/active-directory/governance/review-your-access)