---
title: Руководство. Использование API проверки доступа для проверки доступа к привилегированным ролям
description: Узнайте, как использовать API проверок доступа для периодического просмотра пользователей и групп с доступом к привилегированным ролям, включая активные и подходящие роли.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 845d50d4cd3eb06cf2131f5255567cb4b7861325
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445813"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-privileged-roles"></a>Руководство. Использование API проверки доступа для проверки доступа к привилегированным ролям

API проверок доступа в Microsoft Graph позволяет организациям выполнять аудит и аттестацию доступа, который удостоверения (также называемые субъектами *)* назначаются ресурсам в организации. Одним из наиболее конфиденциальных ресурсов в организации является привилегированные роли. С привилегированной ролью субъект может выполнять административные операции. В зависимости от привилегированной роли некоторые операции могут больше влиять на состояние безопасности организации. С помощью API проверки доступа организации могут периодически проверять субъектов, которые имеют доступ к привилегированным ролям в соответствии с политикой организации.

Contoso Limited — это растущий поставщик услуг, который делегирует различные права администратора Azure AD пользователям, группам и субъектам-службам в организации. Компании необходимо убедиться, что доступ к привилегированным ролям имеют только правильные назначения. Системным аудиторам также следует проверить журнал проверки доступа, чтобы сообщить об эффективности внутренних средств контроля Компании Contoso.

В этом руководстве вы будете использовать API проверок доступа для периодической проверки пользователей и групп с доступом к привилегированным ролям в Contoso. Этот доступ включает как активные, так и допустимые роли.

## <a name="prerequisites"></a>Предварительные требования

Для работы с этим руководством вам потребуются следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5.
+ Войдите в [песочницу Graph от](https://developer.microsoft.com/graph/graph-explorer) имени пользователя с ролью администратора привилегированных ролей.
+ Субъекты с активными или подходящими назначениями привилегированной роли. Эти назначения будут областью проверки доступа. Сведения о назначении привилегированных ролей см. в руководстве по использованию [API управление привилегированными пользователями (PIM) для назначения Azure AD ролей](/graph/tutorial-assign-azureadroles).
    + В этом руководстве роль администратора пользователя является проверяемой ресурсом. Группе безопасности и отдельному пользователю назначена роль.
+ Следующие делегированные разрешения: `AccessReview.ReadWrite.All`.

Чтобы дать согласие на необходимые разрешения в песочнице Graph, скажите следующее:
1. Щелкните значок многоточия по горизонтали справа от сведений об учетной записи пользователя, а затем выберите " **Выбрать разрешения"**.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Microsoft Graph." border="true":::

2. Прокрутите список разрешений для **AccessReview (3),** разверните и выберите .`AccessReview.ReadWrite.All` Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на разрешения Microsoft Graph." border="true":::

>[!NOTE]
>Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости.

## <a name="step-1-create-an-access-review-of-privileged-role-assignments"></a>Шаг 1. Создание проверки доступа для назначений привилегированных ролей

В этом руководстве мы создадим повторяющиеся проверки  доступа для  активных и подходящих назначений роли администратора пользователей. **AccessReviewScheduleDefinition** можно использовать для определения проверки доступа нескольких типов субъектов (пользователей, групп или субъектов-служб) только к одной привилегированной роли. Чтобы проверить доступ к нескольким привилегированным ролям, создайте отдельные **объекты accessReviewScheduleDefinition** .

Следующее определение расписания проверки доступа имеет следующие параметры:

+ Область проверки — это субъекты (**свойство principalScopes** ) с доступом к ресурсу, указанному в свойстве **resourceScopes** . В этом случае субъекты являются группами и пользователями, а ресурс — ролью администратора пользователей.
+ Проверяются как активные, так и допустимые назначения для ресурса роли администратора пользователей.
+ В качестве рецензента выбирается отдельный пользователь. В этом примере вы будете рецензентом.
+ Утверждающий должен предоставить обоснование перед утверждением доступа к привилегированной роли.
+ Решение по умолчанию принимается `None` , когда рецензенты не отвечают на запрос на проверку доступа до истечения срока действия экземпляра.
+ **AutoApplyDecisionsEnabled** не задан и по умолчанию имеет значение `false`. В этом случае после завершения проверки решения не применяются автоматически, поэтому их необходимо применить вручную.
+ Проверка выполняется каждые три месяца в течение трех дней и не будет завершиться.

### <a name="request"></a>Запрос

В следующем запросе замените значение `f674a1c9-4a40-439c-bfa3-4b61a9f29d85` идентификатора пользователя. RoleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` — это глобальный идентификатор шаблона для роли администратора пользователей в Azure AD.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviledroles-create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Review access of users and groups to privileged roles",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph"
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph"
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph"
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "recommendationsEnabled": false,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3
            },
            "range": {
                "type": "noEnd",
                "startDate": "2022-03-02"
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
    "id": "57457d7c-af59-470c-ae71-aa72c657fe0f",
    "displayName": "Review access of users and groups to privileged roles",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "descriptionForReviewers": null,
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": false,
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
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-03-02",
                "endDate": null
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

## <a name="step-2-retrieve-instances-of-the-access-review"></a>Шаг 2. Получение экземпляров проверки доступа

Каждый экземпляр проверки доступа представляет *каждое повторение с каждым уникальным ресурсом* , который находится на проверке. На шаге 1 в области был определен только ресурс роли администратора пользователя. Так как вы определили повторяющиеся проверки доступа, идентификатор экземпляра отличается от идентификатора определения расписания на шаге 1.

### <a name="request"></a>Запрос

В следующем запросе замените `57457d7c-af59-470c-ae71-aa72c657fe0f` значение проверки доступа, созданной на шаге 1.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getinstances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances
```

### <a name="response"></a>Отклик

В этом ответе объект экземпляра отображает дату окончания в виде трех дней после даты начала; Этот период был определен на шаге 1 в свойстве **instanceDurationInDays** объекта **accessReviewScheduleDefinition** . *Возвращается только один экземпляр, представляющий первое повторение только одного проверяемого ресурса.*

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances",
    "@odata.count": 1,
    "value": [
        {
            "id": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "startDateTime": "2022-03-02T15:31:14.607Z",
            "endDateTime": "2022-03-05T15:31:14.607Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
                "principalScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/users",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    },
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/groups",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ],
                "resourceScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ]
            },
            "reviewers": [
                {
                    "query": "/v1.0/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": []
        }
    ]
}
```

Состояние этого экземпляра проверки доступа равно .`InProgress` Состояние `InProgress` означает, что экземпляр проверки открыт для рецензентов для отправки решений, а срок действия этого экземпляра проверки доступа не истек. Вы также получили уведомление по электронной почте от Microsoft Azure с запросом на проверку доступа.

## <a name="step-3-retrieve-access-review-decisions-before-recording-any-decisions"></a>Шаг 3. Получение решений о проверке доступа перед записью любых решений

Прежде чем вы сможете публиковать решения, давайте сначала рассмотрим элементы, ожидающих вашего решения.

### <a name="request"></a>Запрос

В следующем запросе замените следующие значения:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` со значением проверки доступа, созданной на шаге 1.
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` со значением экземпляра проверки доступа, для которого вы хотите получить решения.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getnodecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показаны два элемента принятия решений, каждый из которых соответствует решению для доступа субъекта к ресурсу.

+ Основное свойство показывает, что два участника имеют доступ к роли администратора пользователя — группе С иТ-службе **поддержки (пользователь)** и пользователю **Aline Dupuy**.
+ Значение `NotReviewed` свойства **принятия** решения указывает, что рецензенты не проверяли и не опубликовывали свои решения.
+ Нет доступных рекомендаций, так как рекомендации не были включены в **accessReviewScheduleDefinition** на шаге 1.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
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
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
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
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

Как рецензент вы можете отправлять решения для экземпляра проверки доступа.

## <a name="step-4-record-decisions"></a>Шаг 4. Запись решений

Теперь вы запишите решения для проверки доступа.

Политика компании требует, чтобы доступ к привилегированным ролям был предоставлен только группам, а не отдельным пользователям. В соответствии с политикой компании вы запретите Aline Dupuy доступ при утверждении доступа для группы.

В следующих запросах замените следующие значения:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` со значением проверки доступа, созданной на шаге 1
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` со значением экземпляра проверки доступа, для которого вы хотите получить решения для
+ `4d79fbf6-36e6-430b-ba0a-2a727a480303` со значением экземпляра проверки доступа в области доступа Aline
+ `62fd1c5b-04b8-4703-9fd7-dce6232c3775` со значением экземпляра проверки доступа в области доступа группы ИТ-службы технической поддержки

### <a name="approve-the-security-groups-role-assignment"></a>Утверждение назначения роли группы безопасности

#### <a name="request"></a>Запрос

В следующем запросе вы утверждаете доступ для группы ИТ-службы технической поддержки.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforgroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/62fd1c5b-04b8-4703-9fd7-dce6232c3775
Content-type: application/json

{
    "decision": "Approve",
    "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources"
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

### <a name="deny-the-individual-user-their-role-assignment"></a>Запретить отдельному пользователю назначение роли

#### <a name="request"></a>Запрос

В следующем запросе вы запрещаете доступ для Aline Dupuy.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforuser"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/4d79fbf6-36e6-430b-ba0a-2a727a480303
Content-type: application/json

{
    "decision": "Deny",
    "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

При извлечении решений о проверке доступа (повторите шаг 3) они имеют следующие параметры:
+ Решение о проверке доступа для группы технической поддержки ИТ-службы `Approve` принимается для Aline `Deny`.
+ Объект reviewedBy содержит ваши сведения в качестве рецензента.
+ ApplyResult означает `New` , что решения не были применены.

Хотя вы записали все ожидающие решения для этого экземпляра, решения не были применены к ресурсам и основным объектам. Например, Aline по-прежнему имеет доступ к привилегированной роли. Это назначение можно проверить, выполнив следующий запрос `https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`. Это происходит из-за того, что **параметр autoApplyDecisionsEnabled** `false`был установлен, вы не остановили проверку и период экземпляра не закончился.

В этом руководстве вы не остановите экземпляр вручную, но разрешите его автоматически завершить, а затем применить решения.

> [!TIP]
>
> 1. Пока состояние **экземпляра** проверки доступа не будет помечено `Completed`как " можно изменить решения. Перезапустите шаг 4, чтобы применить различные решения для субъектов.
> 2. Вы также можете вручную остановить экземпляр проверки доступа, чтобы ускорить выполнение до шага 5.

## <a name="step-5-apply-access-review-decisions"></a>Шаг 5. Применение решений для проверки доступа

После установки  `Completed`состояния экземпляра проверки доступа администратор может применить решения.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-applydecisions"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/applyDecisions
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

Теперь Aline теряет доступ к роли администратора пользователей, пока группа ИТ-служб технической поддержки поддерживает доступ. Это состояние назначения ролей можно проверить, выполнив следующий запрос `https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`.

После принятия решений состояние экземпляра проверки  доступа будет следующим`Applied`: Кроме того, так как мы создали повторяющиеся проверки доступа на шаге 1, будет запущен новый экземпляр. Дата начала будет в три месяца с того времени, когда текущий период проверки помечается как завершенный.

## <a name="step-6-retrieve-access-review-decisions"></a>Шаг 6. Получение решений о проверке доступа

Аудиторы Contoso проверяют все решения о предоставлении или запрете доступа к привилегированным ролям в организации. Вы получите журналы принятия решений о проверке доступа для всех проверок доступа с областью действия привилегированных ролей. В этом примере вы получите журналы принятия решений для **accessReviewScheduleDefinition** , созданного на шаге 1.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getdecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Отклик

Следующий объект ответа отличается от объекта ответа, полученного на шаге 3, со следующими параметрами:
+ Решение о проверке **доступа для** службы технической поддержки ИТ-службы `Approve` принимается для Aline `Deny`.
+ Объект **reviewedBy** содержит основные сведения в качестве рецензента.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:50:21.227Z",
            "decision": "Deny",
            "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'",
            "appliedDateTime": "2022-03-02T17:21:05.363Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:31:04.357Z",
            "decision": "Approve",
            "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

<!-- comment this out until a bug is fixed

## Step 7: Retrieve access review history definitions

Contoso's auditors also want to review the access review history for the last quarter. In this example, you'll generate an access review history report for all **accessReviewScheduleDefinition** objects scoped to directory role assignments (roleAssignmentScheduleInstances). In this query, the **decisions** property is empty and therefore defaults to include all decisions in the history report.

First, you'll define the scope of the history report. Then, you generate a download URI that the auditors will use to download the report. The download URI is active for only 24 hours. So, after expiry, you can regenerate another download URI from the previously defined history report.

### Define the scope of the access review history data

In the following request, an empty **decisions** object means all decisions related to the scope of the access review will be included in the history report.

#### Request

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions

{
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "decisions": [],
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "queryType": "MicrosoftGraph",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')"
        }
    ]
}
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/historyDefinitions/$entity",
    "id": "983db508-b77b-427d-ab90-a4041efa658d",
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
    "createdDateTime": "2022-03-02T18:08:51.9032457Z",
    "fulfilledDateTime": null,
    "downloadUri": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

### Retrieve the instances of the access review history

#### Request

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/historyDefinitions('983db508-b77b-427d-ab90-a4041efa658d')/instances",
    "value": [
        {
            "id": "983db508-b77b-427d-ab90-a4041efa658d",
            "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
            "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
            "status": "done",
            "runDateTime": "2022-03-02T18:08:51.9032457Z",
            "fulfilledDateTime": "2022-03-02T18:08:55.8336038Z",
            "downloadUri": null
        }
    ]
}
```

### Generate a link to download the history report from the instance of the access review history

#### Request

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/983db508-b77b-427d-ab90-a4041efa658d/generateDownloadUri()
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#accessReviewHistoryInstance",
    "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
    "id": "a222f18d-5cf5-4210-874c-14d0a7d930b3",
    "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "status": "done",
    "runDateTime": "2022-02-22T10:08:08.2057428Z",
    "fulfilledDateTime": "2022-02-22T10:09:28.5862766Z",
    "downloadUri": "https://ermconsolreportweu.blob.core.windows.net/erm-reports/Last quarter's group reviews April 2021-a222f18d-5cf5-4210-874c-14d0a7d930b3.csv?skoid=4ad0868b-7b78-4869-abb7-8f29151d8428&sktid=33e01921-4d64-4f8c-a055-5bdaffd5e33d&skt=2022-02-22T10:11:22Z&ske=2022-02-22T10:13:22Z&sks=b&skv=2020-04-08&sv=2020-04-08&st=2022-02-22T10:11:22Z&se=2022-02-23T10:11:22Z&sr=b&sp=r&sig=5eX5BfVLS58QqF7oguRH8TeSQdXDHZlapY3y1U%2FGz%2BM%3D"
}
```

The downloadUri property contains a link to download the history report in an Excel file format. This link is active for only 24 hours.

-->
## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Удалите **объект accessReviewScheduleDefinition** , созданный для этого руководства. Так как определение расписания проверки доступа является схемой для проверки доступа, удаление определения приведет к удалению параметров, экземпляров и решений.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-deleteaccessreview"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>Заключение

Вы узнали, как проверить доступ к привилегированным ролям в Azure AD. Ваша организация может использовать API проверок доступа для постоянного управления привилегированным доступом к своим ресурсам, включая роли Azure AD и роли ресурсов Azure. Помимо пользователей и групп, вы также можете проверить доступ приложений и субъектов-служб к привилегированным ролям.

## <a name="see-also"></a>См. также

+ [Справочник по API проверки доступа](/graph/api/resources/accessreviewsv2-root)
+ [Настройка области определения проверки доступа с помощью microsoft API Graph](/graph/accessreviews-scope-concept)
+ [Подробнее об управлении привилегированным доступом](/microsoft-365/compliance/privileged-access-management-overviewe)