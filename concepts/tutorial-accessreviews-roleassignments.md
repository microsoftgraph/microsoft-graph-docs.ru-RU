---
title: Руководство. Используйте API обзоров доступа для просмотра доступа к привилегированным ролям
description: Используйте API обзоров доступа для просмотра доступа к привилегированным ролям
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: adc20b128a56094a0281589d38f9e99b1767b432
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337930"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-privileged-roles"></a>Руководство. Используйте API обзоров доступа для просмотра доступа к привилегированным ролям

API для проверки доступа в Microsoft Graph позволяет организациям проверять и проверять доступ, который удостоверения (также называемые директорами *)* назначены ресурсам организации. Одним из наиболее конфиденциальных ресурсов в организации является привилегированные роли. С привилегированной ролью руководитель может выполнять административные операции. В зависимости от привилегированной роли некоторые операции могут иметь большее влияние на положение безопасности организации. С помощью API отзывов о доступе организации могут периодически засвидетельстовки для директоров, которые имеют доступ к привилегированным ролям в политике организации.

Contoso Limited — это растущий поставщик услуг, который делегировал различные привилегии администратора Azure AD пользователям, группам и директорам служб в организации. Компании необходимо обеспечить доступ только к привилегированным ролям только для правильных назначаемой должности. Аудиторам системы также следует проверять историю проверки доступа, чтобы сообщить об эффективности внутренних элементов управления Contoso.

В этом руководстве API обзоров доступа используется для периодических обзоров пользователей и групп с доступом к привилегированным ролям в Contoso. Этот доступ включает как активные, так и подходящие роли.

## <a name="prerequisites"></a>Необходимые компоненты

Для завершения этого руководства необходимы следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5.
+ Вопишите Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя в роли администратора привилегированных ролей.
+ Директора с активными или подходящими назначениями на привилегированную роль. Эти назначения будут областью обзора доступа. Чтобы назначить привилегированные роли, см. в руководстве[: используйте API управление привилегированными пользователями (PIM) для назначения ролей Azure AD](/graph/tutorial-assign-azureadroles).
    + В этом руководстве роль администратора пользователя — это ресурс в обзоре. Группе безопасности и отдельному пользователю назначена роль.
+ Следующие делегированные разрешения: `AccessReview.ReadWrite.All`.

Согласие на необходимые разрешения в Graph Explorer:
1. Выберите значок горизонтальных эллипсов справа от сведений учетной записи пользователя, а затем выберите **выбранные разрешения**.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Выберите разрешения Graph Microsoft." border="true":::

2. Прокрутите список разрешений **для AccessReview (3)**, разйдите и выберите `AccessReview.ReadWrite.All`. Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Согласие на Graph разрешений Майкрософт." border="true":::

>[!NOTE]
>Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.

## <a name="step-1-create-an-access-review-of-privileged-role-assignments"></a>Шаг 1. Создание обзора доступа к привилегированным назначениям ролей

В этом руководстве мы создадим повторяющиеся обзоры  доступа как  активных, так и подходящих назначений на роль администратора пользователей. **AccessReviewScheduleDefinition** можно использовать для определения обзора доступа нескольких основных типов (пользователей и групп или директоров служб) только для одной привилегированной роли. Чтобы просмотреть доступ к нескольким привилегированным ролям, создайте отдельные **объекты accessReviewScheduleDefinition** .

В следующем определении расписания проверки доступа параметров:

+ Областью обзора являются директора (**свойство principalScopes** ) с доступом к ресурсу, указанному в **свойстве resourceScopes** . В этом случае основными пользователями являются как группы, так и пользователи, а ресурс — роль администратора пользователя.
+ Рассматриваются как активные, так и подходящие назначения для ресурса ролей администратора пользователей.
+ Отдельный пользователь выбирается в качестве рецензента. В этом примере вы будете рецензентом.
+ Перед утверждением доступа к привилегированной роли утвердитель должен предоставить обоснование.
+ Решение по умолчанию принимается `None` в том случае, если рецензенты не отвечают на запрос на проверку доступа до истечения срока действия экземпляра.
+ **autoApplyDecisionsEnabled** не задаваемый и по умолчанию `false`. В этом случае после завершения проверки решения не применяются автоматически, поэтому их необходимо применять вручную.
+ Проверка повторяется каждые три месяца в течение трех дней и не заканчивается.

### <a name="request"></a>Запрос

В следующем запросе замените `f674a1c9-4a40-439c-bfa3-4b61a9f29d85` значение вашего пользовательского ИД. RoleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` — это глобальный идентификатор шаблона для роли администратора пользователей в Azure AD.

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
                "query": "/roleManagement/directory/roleDefinitions/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
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

## <a name="step-2-retrieve-instances-of-the-access-review"></a>Шаг 2. Извлечение экземпляров обзора доступа

Каждый экземпляр обзора доступа представляет *каждое повторение с каждым уникальным ресурсом* , который находится на рассмотрении. На шаге 1 в области был определен только ресурс ролей администратора пользователя. Так как вы определили повторяющийся обзор доступа, ID экземпляра отличается от ID определения расписания в шаге 1.

### <a name="request"></a>Запрос

В следующем запросе замените `57457d7c-af59-470c-ae71-aa72c657fe0f` значение обзора доступа, созданного в шаге 1.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getinstances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances
```

### <a name="response"></a>Отклик

В этом ответе объект экземпляра показывает даты окончания через три дня после даты начала; этот период был определен в шаге 1 в **свойстве instanceDurationInDays** объекта **accessReviewScheduleDefinition** . *Возвращается только один экземпляр, представляющий первое повторение только одного просматриваемого ресурса.*

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

Состояние этого экземпляра обзора доступа .`InProgress` Состояние `InProgress` означает, что экземпляр проверки открыт для отправки решений рецензентами, и период для этого экземпляра проверки доступа не истек. Кроме того, вы получили уведомление по электронной почте от Microsoft Azure с просьбой выполнить проверку доступа.

## <a name="step-3-retrieve-access-review-decisions-before-recording-any-decisions"></a>Шаг 3. Извлечение решений по обзору доступа перед записью любых решений

Прежде чем вы сможете вывешить решения, сначала проинспектировать элементы, ожидающих вашего решения.

### <a name="request"></a>Запрос

В следующем запросе замените следующие значения:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` со значением обзора доступа, созданного в шаге 1.
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` со значением экземпляра обзора доступа, для который вы хотите получить решения.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getnodecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Отклик

В следующем ответе показано два пункта решения, каждый из которых соответствует решению для доступа к ресурсу.

+ Основное свойство показывает, что два директора имеют доступ к роли администратора пользователя— группе С ИТ-помощником **(пользователь)** и пользователем С именем **Aline Dupuy**.
+ Значение `NotReviewed` свойства **решения** указывает на то, что рецензенты не рассмотрели и не опубликовали свои решения.
+ Рекомендации недоступны, так как рекомендации не были включены в **accessReviewScheduleDefinition** в шаге 1.

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

В качестве рецензента теперь можно отправлять решения для экземпляра обзора доступа.

## <a name="step-4-record-decisions"></a>Шаг 4. Запись решений

Теперь вы будете записывать решения для проверки доступа.

Политика компании требует, чтобы доступ к привилегированным ролям был предоставлен только группам, а не отдельным пользователям. В соответствии с политикой компании при одобрении доступа для группы будет отсутствить доступ к Aline Dupuy.

В следующих запросах замените следующие значения:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` со значением обзора доступа, созданного в шаге 1
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` со значением экземпляра обзора доступа, который вы хотите получить для получения решений для
+ `4d79fbf6-36e6-430b-ba0a-2a727a480303` со значением экземпляра обзора доступа к доступу Aline
+ `62fd1c5b-04b8-4703-9fd7-dce6232c3775` значение экземпляра проверки доступа к доступу группы ИТ-помощников

### <a name="approve-the-security-groups-role-assignment"></a>Утверждение назначения ролей группы безопасности

#### <a name="request"></a>Запрос

В следующем запросе вы утверждаете доступ для группы ИТ-помощников.

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

### <a name="deny-the-individual-user-their-role-assignment"></a>Запретить отдельному пользователю назначение ролей

#### <a name="request"></a>Запрос

В следующем запросе вы отказываете в доступе для Aline Dupuy.

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

При извлечении решений по обзору доступа (повторите шаг 3) у них есть следующие параметры:
+ Решение о проверке доступа для группы ИТ-помощников `Approve` принимается в то время как для Aline это `Deny`.
+ Объект reviewedBy содержит ваши сведения в качестве рецензента.
+ ApplyResult означает `New` , что решения не были применены.

Хотя вы зафиксировали все ожидающих решений для этого экземпляра, решения не были применены к ресурсу и основным объектам. Например, У Aline по-прежнему есть доступ к привилегированной роли. Вы можете проверить это назначение, запуская следующий запрос `https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`. Это поведение, так как **для autoApplyDecisionsEnabled** `false`было установлено, что обзор не был остановлен, и период экземпляра не закончился.

В этом руководстве вы не остановите экземпляр вручную, но вы позволите ему автоматически закончиться, а затем применить решения.

> [!TIP]
>
> 1. До тех **пор,** пока состояние экземпляра обзора доступа не будет помечено как `Completed`, можно изменить решения. Перезапев шаг 4 для применения различных решений для директоров.
> 2. Вы также можете вручную остановить экземпляр проверки доступа, чтобы ускорить процесс выполнения до 5-го шага.

## <a name="step-5-apply-access-review-decisions"></a>Шаг 5. Применение решений по обзору доступа

В качестве администратора после **того**`Completed`, как установлено состояние экземпляра проверки доступа, вы можете применить решения.

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

Теперь Aline потеряла доступ к роли администратора пользователей, а группа it helpdesk сохранила доступ. Вы можете проверить это состояние назначения ролей, запуская следующий запрос `https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`.

После того как решения будут применены, **состояние экземпляра** проверки доступа будет .`Applied` Кроме того, поскольку в шаге 1 создан повторяющийся обзор доступа, будет запущен новый экземпляр. Его дата начала — три месяца с момента окончания текущего периода проверки.

## <a name="step-6-retrieve-access-review-decisions"></a>Шаг 6. Извлечение решений по обзору доступа

Аудиторы Contoso рассматривают все решения о предоставлении или отказе в доступе к привилегированным ролям в организации. Вы получите журналы принятия решений о просмотре доступа для всех обзоров доступа, доступных для привилегированных ролей. В этом примере вы получите журналы решений для созданного в шаге 1 **accessReviewScheduleDefinition** .

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getdecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Отклик

Следующий объект ответа отличается от объекта отклика, полученного в шаге 3 со следующими настройками:
+ Решение о проверке **доступа** для ИТ-помощников `Approve` принимается в то время как для Aline это `Deny`.
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
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/historyDefinitions/$entity",
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
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/historyDefinitions('983db508-b77b-427d-ab90-a4041efa658d')/instances",
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
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances/983db508-b77b-427d-ab90-a4041efa658d/generateDownloadUri()
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewHistoryInstance",
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

Удалите **объект accessReviewScheduleDefinition** , созданный для этого руководства. Так как определение расписания проверки доступа является планом обзора доступа, удаление определения удаляет параметры, экземпляры, решения.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-deleteaccessreview"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
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

Вы узнали, как просмотреть доступ к привилегированным ролям в Azure AD. Ваша организация может использовать API обзоров доступа для непрерывного управления привилегированным доступом к своим ресурсам, включая роли Azure AD и роли ресурсов Azure. Помимо пользователей и групп, вы также можете просмотреть доступ приложений и директоров служб к привилегированным ролям.

## <a name="see-also"></a>См. также

+ [Ссылка на API обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [Настройка области определения обзора доступа с помощью API microsoft Graph](/graph/accessreviews-scope-concept)
+ [Подробнее об управлении привилегированным доступом](/microsoft-365/compliance/privileged-access-management-overviewe)