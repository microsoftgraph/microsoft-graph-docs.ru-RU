---
title: Руководство. Использование API управление привилегированными пользователями (PIM) для назначения Azure AD ролей
description: Узнайте, как использовать API управление привилегированными пользователями (PIM) в Microsoft Graph для назначения Azure AD привилегированных ролей.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 78e523a12d59ac7b25482da26f3fb594e9517657
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247192"
---
# <a name="tutorial-use-the-privileged-identity-management-pim-api-to-assign-azure-ad-roles"></a>Руководство. Использование API управление привилегированными пользователями (PIM) для назначения Azure AD ролей

Microsoft Graph API PIM позволяет организациям управлять привилегированным доступом к ресурсам в Azure Active Directory (Azure AD). Он также помогает управлять рисками привилегированного доступа путем ограничения активности доступа, управления областью доступа и предоставления доступного для аудита журнала привилегированного доступа.

В этом руководстве вымышленная компания Contoso Limited хочет, чтобы служба ИТ-поддержки управляет жизненным циклом доступа сотрудников. Компания определила роль Azure AD пользователя как соответствующую привилегированную роль, необходимую службе технической поддержки ИТ, и будет использовать API PIM для назначения роли.

Вы создадите группу безопасности, назначаемую ролем, для ИТ-службы технической поддержки и с помощью API PIM назначьте группе безопасности право на роль администратора пользователей. Назначая допустимую роль группе безопасности, contoso имеет более эффективный способ управления доступом администратора к ресурсам, таким как Azure AD ролей. Например:

+ При удалении существующих или добавлении дополнительных членов группы также удаляются администраторы.
+ Добавление дополнительных ролей для участников группы вместо назначения ролей отдельным пользователям.

Назначение прав доступа вместо постоянного активного права администратора пользователей позволяет компании принудительно применять **JIT-доступ**, который предоставляет временные разрешения на выполнение привилегированных задач. После определения допустимости роли соответствующий член группы активирует свое назначение на временный период. Все записи об активации ролей будут доступны для аудита в компании.

>[!NOTE]
>Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости.

## <a name="prerequisites"></a>Необходимые условия

Для работы с этим руководством вам потребуются следующие ресурсы и привилегии:

+ Рабочий клиент Azure AD с включенной Azure AD Premium P2 или EMS E5.
+ Войдите в [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя с ролью глобального администратора.
  + [Необязательно] Запустите новый сеанс инкогнито или браузера InPrivate или запустите сеанс в анонимном браузере. Вы выполните вход позже в этом руководстве.
+ Следующие делегированные разрешения: `User.ReadWrite.All`, `Group.ReadWrite.All`, `Directory.Read.All`, , `RoleEligibilitySchedule.ReadWrite.Directory`и `RoleAssignmentSchedule.ReadWrite.Directory`, и `RoleManagement.ReadWrite.Directory`.
+ Authenticator приложение, установленное на телефоне, чтобы зарегистрировать пользователя для многофакторной проверки подлинности (MFA).

Чтобы дать согласие на необходимые разрешения в Graph Explorer:
1. Щелкните значок многоточия по горизонтали справа от сведений об учетной записи пользователя, а затем выберите " **Выбрать разрешения"**.
  
      :::image type="content" source="/graph/images/GE-Permissions/selectpermissions.png" alt-text="Выберите разрешения Graph Майкрософт." border="true":::

2. Прокрутите список разрешений до следующих разрешений:
    + Группу (2), разверните и выберите **Group.ReadWrite.All**.
    + Разверните каталог (4), а затем выберите **Directory.Read.All**.
    + RoleAssignmentSchedule (2), разверните и выберите **RoleAssignmentSchedule.ReadWrite.Directory**.
    + RoleEligibilitySchedule (2), разверните и выберите **RoleEligibilitySchedule.ReadWrite.Directory**.
    + RoleManagement (3), разверните и выберите **RoleManagement.ReadWrite.Directory**.
    + Пользователь (8), разверните и выберите **User.ReadWrite.All**.
   
   Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Для получения `RoleEligibilitySchedule.ReadWrite.Directory` разрешений `RoleAssignmentSchedule.ReadWrite.All` и разрешений согласие от имени вашей организации.

      :::image type="content" source="/graph/images/GE-Permissions/User.ReadWrite.All-consent.png" alt-text="Предоставление согласия на Graph майкрософт." border="true":::

## <a name="step-1-create-a-test-user"></a>Шаг 1. Создание тестового пользователя

Создайте пользователя, который должен сбросить пароль при первом входе. На этом шаге запишите значение идентификатора нового пользователя для использования  на следующем шаге. После создания пользователя посетите веб-портал Azure и включите многофакторную проверку подлинности (MFA) для пользователя. Дополнительные сведения о включении MFA см. в [разделе "См. также](#see-also) ".


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

## <a name="step-2-create-a-security-group-that-can-be-assigned-an-azure-ad-role"></a>Шаг 2. Создание группы безопасности, которая может быть назначена Azure AD роли

Создайте группу, которая может быть назначена Azure AD роли. Назначьте себя владельцем группы и вас и Aline (пользователя, созданного на шаге 1) в качестве участников.

### <a name="request-create-a-role-assignable-group"></a>Запрос. Создание группы с возможностью назначения ролей

Замените `1ed8ac56-4827-4733-8f80-86adc2e67db5` идентификатор и `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` значение идентификатора Aline.

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
    ],
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

## <a name="step-3-create-a-unifiedroleeligibilityschedulerequest"></a>Шаг 3. Создание unifiedRoleEligibilityScheduleRequest

Теперь, когда у вас есть группа безопасности, назначьте ее в качестве подходящей для роли администратора пользователей. На этом шаге:

+ Создайте объект unifiedRoleEligibilityScheduleRequest, который определяет группу **ИТ-службы технической поддержки (пользователя)** в качестве подходящей для роли администратора пользователя в течение одного года. Azure AD это допустимое назначение распространяется на участников группы, то есть вас и Алин.
+ Окажите допустимое назначение для всего клиента. Это позволяет администратору пользователя использовать свои привилегии для всех пользователей в клиенте, за исключением пользователей с более высоким уровнем привилегий, таких как глобальный администратор.

### <a name="request"></a>Запрос

Замените `e77cbb23-0ff2-4e18-819c-690f58269752` значение идентификатора группы  безопасности **ИТ-службы (** пользователя). Этот **principalId** определяет получателя прав на роль администратора пользователя. RoleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` — это глобальный идентификатор шаблона для роли администратора пользователей в Azure AD.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-unifiedRoleEligibilityScheduleRequest_create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
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

Хотя участники группы теперь имеют право на роль администратора пользователей, они по-прежнему не могут использовать эту роль. Это связано с тем, что они еще не активируют свое право на участие. Это можно проверить, проверив текущие назначения ролей пользователя.


### <a name="request"></a>Запрос

В следующем запросе замените `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` значение идентификатора Aline **.**

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignments_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignments",
    "value": []
}
```

Пустой объект ответа показывает, что у Aline нет Azure AD ролей в Contoso. Теперь Aline активирует доступную роль администратора пользователей в течение ограниченного времени.

## <a name="step-5-user-self-activates-their-eligible-assignment"></a>Шаг 5. Пользователь самостоятельно активирует свое подходящее назначение

Запрос на инцидент CONTOSO: security-012345 был вызван в системе управления инцидентами Компании Contoso, и компания требует, чтобы все маркеры обновления сотрудника были недействительными. Как член службы технической поддержки ИТ,Aline отвечает за выполнение этой задачи.

Сначала запустите приложение Authenticator на телефоне и откройте учетную запись Aline Dupuy.

Войдите в Graph Explorer в качестве Aline. Для этого шага можно использовать сеанс инкогнито или анонимный браузер. Таким образом, вы не будете прерывать текущий сеанс как пользователь с ролью глобального администратора. Кроме того, можно прервать текущий сеанс, выполнив выход из Graph Explorer и снова войдя в систему как Aline.

Вошед в систему как Aline, вы сначала измените пароль, так как он был указан во время создания учетной записи. После этого, так как администратор настроит учетную запись для многофакторной проверки подлинности, вам будет предложено настроить учетную запись в приложении Authenticator и получить запрос на вход в MFA. Это связано с тем, что PIM требует многофакторную проверку подлинности для всех активных назначений ролей.

После входа активируйте роль администратора пользователя в течение пяти часов.

### <a name="request"></a>Запрос

Чтобы активировать роль, вызовите конечную `roleAssignmentScheduleRequests` точку. В этом запросе действие `UserActivate` позволяет активировать допустимое назначение в течение пяти часов.

+ Для **principalId** укажите значение идентификатора (Aline's **).**
+ **RoleDefinitionId** — это **идентификатор** роли, на которую вы имеете право, в данном случае роль администратора пользователя.
+ Введите сведения о системе запросов, которая предоставляет обоснование для аудита для активации запроса.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignmentScheduleRequests_selfActivate"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
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

Вы можете подтвердить назначение, выполнив команду `GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')`. Объект ответа возвращает только что активированное назначение роли с состоянием " `Granted`. С новыми привилегиями выполните все разрешенные действия в течение пяти часов, для выполнения задания. Это включает в себя недействительные маркеры обновления всех сотрудников. По истечении пяти часов срок действия активного назначения истекает, но благодаря членству в группе ИТ-поддержки **(пользователи)** вы по-прежнему можете использовать роль администратора пользователей.

Вернув сеанс глобального администратора, вы получили уведомления о допустимом назначении и активации роли. Это позволяет глобальному администратору быть в курсе всех прав администратора в вашей организации.

## <a name="step-6-clean-up-resources"></a>Шаг 6. Очистка ресурсов

Войдите в систему с правами глобального администратора и удалите следующие ресурсы, созданные для этого руководства: запрос на получение прав на роль, группа ИТ-поддержки (пользователи) и тестовый пользователь (Aline Dupuy).

### <a name="revoke-the-role-eligibility-request"></a>Отзыв запроса на получение прав на роль

#### <a name="request"></a>Запрос

Замените `e77cbb23-0ff2-4e18-819c-690f58269752` **идентификатором группы** ИТ-поддержки (пользователи).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleEligibilityScheduleRequests_revoke"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "dcd11a1c-300f-4d17-8c7a-523830400ec8",
    "status": "Revoked",
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}
```

### <a name="delete-the-it-support-users-group"></a>Удаление группы ИТ-поддержки (пользователи)

#### <a name="request"></a>Запрос

Замените `e77cbb23-0ff2-4e18-819c-690f58269752` **идентификатором группы** ИТ-поддержки (пользователи).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-group_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/groups/e77cbb23-0ff2-4e18-819c-690f58269752
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

Замените `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` значение идентификатора Aline **.**

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-user_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2
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

+ [Общие сведения об управлении ролами с помощью PIM](/graph/api/resources/privilegedidentitymanagementv3-overview)
+ [Azure AD встроенных ролей](/azure/active-directory/roles/permissions-reference#all-roles)
+ [Включение многофакторной Azure AD проверки подлинности для каждого пользователя для защиты событий входа](/azure/active-directory/authentication/howto-mfa-userstates)
+ [Тип ресурса unifiedRoleEligibilityScheduleRequest](/graph/api/resources/unifiedroleeligibilityschedulerequest)