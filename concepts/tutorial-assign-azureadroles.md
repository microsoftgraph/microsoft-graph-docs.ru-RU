---
title: Руководство. Используйте API управление привилегированными пользователями (PIM) для назначения ролей Azure AD
description: Узнайте, как использовать API управление привилегированными пользователями (PIM) в Microsoft Graph для назначения привилегированных ролей Azure AD.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 9f706b6c8a39548fb65dcb46e83845b51fd9af21
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777308"
---
# <a name="tutorial-use-the-privileged-identity-management-pim-api-to-assign-azure-ad-roles"></a>Руководство. Используйте API управление привилегированными пользователями (PIM) для назначения ролей Azure AD

API Graph майкрософт позволяет организациям управлять привилегированным доступом к ресурсам в Azure Active Directory (Azure AD). Это также помогает управлять рисками привилегированного доступа, ограничив время активного доступа, управляя областью доступа и предоставляя аудитируемый журнал привилегированного доступа.

В этом руководстве вымышлетельная компания Contoso Limited желает, чтобы ее ИТ-службы помогли управлять жизненным циклом доступа сотрудников. Компания определила роль администратора пользователя Azure AD в качестве соответствующей привилегированной роли, требуемой службой it helpdesk, и будет использовать API PIM для назначения роли.

Вы создаите группу безопасности, назначимую роли для ИТ-службы helpdesk, и с помощью API PIM назначите группе безопасности право на роль администратора пользователя. Назначив подходящую роль группе безопасности, Contoso имеет более эффективный способ управления доступом администратора к ресурсам, таким как роли Azure AD. Например:

+ Удаление существующих или добавление дополнительных членов группы также удаляет администраторов.
+ Добавление дополнительных ролей участникам группы вместо назначения ролей отдельным пользователям.

Назначение права вместо постоянно активной привилегии администратора пользователей позволяет компании обеспечить доступ к простому **времени,** что дает временные разрешения на выполнение привилегированных задач. После определения права на роль соответствующий член группы активирует свое назначение на временный период. Все записи активаций ролей будут проверяться компанией.

>[!NOTE]
>Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.

## <a name="prerequisites"></a>Необходимые условия

Для завершения этого руководства необходимы следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или emS E5.
+ Вопишитесь [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя в роли глобального администратора.
  + [Необязательный] Запустите новый сеанс инкогнито или браузера InPrivate или запустите сеанс в анонимном браузере. Далее в этом учебнике вы вопишитесь.
+ Следующие делегированные разрешения: `User.ReadWrite.All` , , , и , и `Group.ReadWrite.All` `Directory.Read.All` `RoleEligibilitySchedule.ReadWrite.Directory` `RoleAssignmentSchedule.ReadWrite.Directory` `RoleManagement.ReadWrite.Directory` .
+ Authenticator установлено на телефоне для регистрации пользователя для многофакторной проверки подлинности (MFA).

Согласие на необходимые разрешения в Graph Explorer:
1. Выберите значок горизонтальных эллипсов справа от сведений учетной записи пользователя, а затем выберите **Выберите разрешения.**
  
      :::image type="content" source="/graph/images/GE-Permissions/selectpermissions.png" alt-text="Выберите разрешения Graph Microsoft." border="true":::

2. Прокрутите список разрешений для этих разрешений:
    + Группа (2), развиньте и выберите **Group.ReadWrite.All**.
    + Каталог (4), расширить и затем выбрать **Directory.Read.All**.
    + RoleAssignmentSchedule (2), расширяйте и выберите **RoleAssignmentSchedule.ReadWrite.Directory**.
    + RoleEligibilitySchedule (2), расширяйте и выберите **RoleEligibilitySchedule.ReadWrite.Directory**.
    + RoleManagement (3), развиньте и выберите **RoleManagement.ReadWrite.Directory**.
    + Пользователь (8), расширить и затем выбрать **User.ReadWrite.All**.
   
   Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Для получения `RoleEligibilitySchedule.ReadWrite.Directory` `RoleAssignmentSchedule.ReadWrite.All` разрешений и разрешений согласие от имени организации.

      :::image type="content" source="/graph/images/GE-Permissions/User.ReadWrite.All-consent.png" alt-text="Согласие на Graph разрешений Майкрософт." border="true":::

## <a name="step-1-create-a-test-user"></a>Шаг 1. Создание тестового пользователя

Создайте пользователя, который должен сбросить пароль при первом входе. На этом шаге зафиксировать значение **id** нового пользователя для использования на следующем шаге. После создания пользователя посетите портал Azure и ввести для пользователя многофакторную проверку подлинности (MFA). Дополнительные сведения о включаемой MFA см. в разделе [See also.](#see-also)


### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@Contoso.com",
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
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2/Microsoft.DirectoryServices.User",
    "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-that-can-be-assigned-an-azure-ad-role"></a>Шаг 2. Создание группы безопасности, которая может быть назначена роли Azure AD

Создайте группу, которая назначается роли Azure AD. Назначьте себя владельцем группы, а вы и Aline (пользователь, созданный в шаге 1) в качестве участников.

### <a name="request-create-a-role-assignable-group"></a>Запрос. Создайте группу, назначаемую для ролей

`1ed8ac56-4827-4733-8f80-86adc2e67db5`Замените **свой id**.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createSecurityGroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "isAssignableToRole": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5"
    ]
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/e77cbb23-0ff2-4e18-819c-690f58269752/Microsoft.DirectoryServices.Group",
    "id": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "groupTypes": [],
    "isAssignableToRole": true,
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-3883711267-1310199794-258579585-1385637464",
    "visibility": "Private",
    "onPremisesProvisioningErrors": []
}
```

### <a name="request"></a>Запрос

Назначьте себя и Aline в качестве двух членов группы безопасности. В следующем запросе замените:
+ `e77cbb23-0ff2-4e18-819c-690f58269752`в URL-адресе со значением **id группы.**
+ `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` со значением **ID** Aline.
+ `1ed8ac56-4827-4733-8f80-86adc2e67db5` со значением **вашего id**.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-addGroupMembers"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groups/e77cbb23-0ff2-4e18-819c-690f58269752
Content-type: application/json

{
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
        "https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
    ]
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```
HTTP/1.1 204 No Content
```

## <a name="step-3-create-a-unifiedroleeligibilityschedulerequest"></a>Шаг 3. Создание единой системыRoleEligibilityScheduleRequest

Теперь, когда у вас есть группа безопасности, назначьте ее в качестве подходящих для роли администратора пользователей. На этом шаге:

+ Создайте объект unifiedRoleEligibilityScheduleRequest, который определяет группу **it helpdesk (User)** в качестве права на роль администратора пользователя в течение одного года. Azure AD распространяет это назначение на членов группы, то есть на вас и на Aline.
+ Область назначения, находящегося на 1000 000 000 000 00 Это позволяет администратору пользователя использовать свои привилегии для всех пользователей в клиенте, за исключением более высоких привилегированных пользователей, таких как Глобальный администратор.

### <a name="request"></a>Запрос

Замените значение id группы безопасности `e77cbb23-0ff2-4e18-819c-690f58269752` **ИТ-службы helpdesk (User).**  Этот **principalId** определяет назначителем права на роль администратора пользователя. RoleDefinitionId — это глобальный идентификатор шаблона `fe930be7-5e62-47db-91af-98c3a49a38b1` для роли администратора пользователей в Azure AD.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-unifiedRoleEligibilityScheduleRequest_create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminAssign",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "scheduleInfo": {
        "startDateTime": "2021-07-01T00:00:00Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequests"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "status": "Provisioned",
    "createdDateTime": "2021-09-03T20:45:28.3848182Z",
    "completedDateTime": "2021-09-03T20:45:39.1194292Z",
    "action": "AdminAssign",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "user": {
            "id": "1ed8ac56-4827-4733-8f80-86adc2e67db5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-03T20:45:39.1194292Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z"
        }
    },
    "ticketInfo": {}
}
```

## <a name="step-4-confirm-the-users-current-role-assignments"></a>Шаг 4. Подтверждение текущих назначений ролей пользователя

Хотя теперь члены группы имеют право на роль администратора пользователей, они по-прежнему не могут использовать эту роль. Это потому, что они еще не активировать свои права. Вы можете подтвердить, проверив текущие назначения ролей пользователя.


### <a name="request"></a>Запрос

В следующем запросе замените значение `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` **ID** Aline.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignments_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignments"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": []
}
```

На пустом объекте ответа показано, что у Aline нет существующих ролей Azure AD в Contoso. Теперь Aline активирует свою роль администратора пользователей в течение ограниченного времени.

## <a name="step-5-user-self-activates-their-eligible-assignment"></a>Шаг 5. Пользователь самостоятельно активирует свое назначение

Билет на инцидент CONTOSO: Security-012345 был поднят в системе управления инцидентами Contoso, и компания требует, чтобы все маркеры обновления сотрудника были признаны недействительными. Как член it-helpdesk, Aline отвечает за выполнение этой задачи.

Сначала запустите приложение Authenticator на телефоне и откройте учетную запись Aline Dupuy.

Во входе Graph Explorer в качестве Aline. Для этого шага можно использовать сеанс инкогнито или анонимный браузер. Таким образом, текущий сеанс в роли глобального администратора не прерывается. Кроме того, вы можете прервать текущий сеанс, подписав Graph Explorer и вернувшись в качестве Aline.

Во время создания учетной записи вы сначала измените пароль, так как он был указан в качестве Aline. Затем, так как администратор настроил учетную запись для MFA, вам будет предложено настроить учетную запись в приложении Authenticator и получить вызов для регистрации MFA. Это потому, что PIM требует, чтобы MFA для всех назначений активной роли.

После регистрации активируйте роль администратора пользователя в течение пяти часов.

### <a name="request"></a>Запрос

Чтобы активировать роль, позвоните в `roleAssignmentScheduleRequests` конечную точку. В этом запросе действие позволяет активировать допустимые назначения, в этом `UserActivate` случае в течение пяти часов.

+ Для **principalId** поставляем значение **id**(Aline's).
+ **RoleDefinitionId** — это **id** роли, на которую вы имеете право, в данном случае на роль администратора пользователей.
+ Введите сведения о системе билетов, которая обеспечивает проверку для активации запроса.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignmentScheduleRequests_selfActivate"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
Content-type: application/json

{
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "status": "Granted",
    "createdDateTime": "2021-09-03T21:10:49.6670479Z",
    "completedDateTime": "2021-09-04T15:13:00Z",
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "createdBy": {
        "user": {
            "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00Z",
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

Вы можете подтвердить назначение, запуская `GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')` . Объект ответа возвращает вновь активированное назначение роли со своим значением состояния `Granted` . С помощью новой привилегии выполнять любые разрешенные действия в течение пяти часов, для выполнения задания. Это включает недействительные маркеры обновления всех сотрудников. По истечении пяти часов срок действия активного назначения истекает, но благодаря вашему членству в группе ИТ-поддержки **(пользователей)** вы по-прежнему можете претендовать на роль администратора пользователя.

Во время глобального сеанса администратора вы получили уведомления как о назначении, так и об активации роли. Это позволяет глобальному администратору быть в курсе всех возвышения к привилегиям администратора в вашей организации.

## <a name="step-6-clean-up-resources"></a>Шаг 6. Очистка ресурсов

Впишитесь в качестве глобального администратора и удалите следующие ресурсы, созданные для этого руководства: запрос на получение права на роль, группу ИТ-поддержки (пользователи) и тестовый пользователь (Aline Dupuy).

### <a name="revoke-the-role-eligibility-request"></a>Отопросить запрос на право на роль

#### <a name="request"></a>Запрос

`e77cbb23-0ff2-4e18-819c-690f58269752`Замените **id** группы ИТ-поддержки (пользователей).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleEligibilityScheduleRequests_revoke"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}

```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "dcd11a1c-300f-4d17-8c7a-523830400ec8",
    "status": "Revoked",
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}
```

### <a name="delete-the-it-support-users-group"></a>Удаление группы ИТ-поддержки (пользователей)

#### <a name="request"></a>Запрос

`e77cbb23-0ff2-4e18-819c-690f58269752`Замените **id** группы ИТ-поддержки (пользователей).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-group_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/groups/e77cbb23-0ff2-4e18-819c-690f58269752
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-test-user"></a>Удаление тестового пользователя

#### <a name="request"></a>Запрос

Замените `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` значение **ID** Aline.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-user_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>См. также

+ [Начните использовать управление привилегированными пользователями](/azure/active-directory/privileged-identity-management/pim-getting-started)
+ [Роли, встроенные в Azure AD](/azure/active-directory/roles/permissions-reference#all-roles)
+ [Включить многофакторную проверку подлинности Azure AD для обеспечения безопасности событий регистрации](/azure/active-directory/authentication/howto-mfa-userstates)
+ [тип ресурса unifiedRoleEligibilityScheduleRequest](/graph/api/resources/unifiedroleeligibilityschedulerequest?view=graph-rest-beta&preserve-view=true)