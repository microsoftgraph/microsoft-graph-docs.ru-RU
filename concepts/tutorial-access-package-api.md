---
title: Учебник. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Microsoft Graph
description: Узнайте, как управлять доступом к ресурсам в управлении правами Active Directory (Azure AD) с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae9dfec7ae5db453ff6962ffd5684dd3bd9ee7d1
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271864"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a>Учебник. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Microsoft Graph

Управление доступом ко всем ресурсам, которые требуются сотрудникам, например группам, приложениям и сайтам, является важной функцией для организаций. Вы хотите предоставить сотрудникам нужный уровень доступа, необходимый им для продуктивной работы, и удалить их доступ, когда он больше не нужен. [Управление правами Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) с помощью API Microsoft Graph позволяет управлять этим типом доступа.

В этом руководстве вам было предложено разработать код для создания пакета ресурсов для маркетинговой кампании, которые внутренние пользователи могут самостоятельно запрашивать. Запросы не требуют утверждения, а срок действия доступа пользователя истекает через 30 дней. В этом руководстве ресурсы маркетинговой кампании являются только членством в одной группе, но это может быть коллекция групп, приложений или сайтов SharePoint Online.

>**Примечание.** Объекты ответа, показанные в этом руководстве, могут быть сокращены для учитаемости. 

## <a name="prerequisites"></a>Необходимые компоненты

Чтобы успешно выполнить это руководство, убедитесь, что у вас есть необходимые условия:
- Для управления правами Azure AD требуются определенные лицензии. Дополнительные сведения [см. в требованиях к лицензиям.](/azure/active-directory/governance/entitlement-management-overview#license-requirements) В клиенте требуются следующие лицензии:
    - Azure AD Premium P2
    - Лицензия на Enterprise Mobility + Security (EMS) E5
- В этом руководстве предполагается, что вы используете проводник Microsoft Graph, но можете использовать Postman или создать собственное клиентские приложения для вызова Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, необходимо использовать учетную запись с ролью глобального администратора и соответствующими разрешениями. Для этого учебника необходимы `User.ReadWrite.All` `Group.ReadWrite.All` делегированная `EntitlementManagement.ReadWrite.All` и делегированная разрешения. Чтобы настроить разрешения в проводнике Microsoft Graph, выполните следующие действия.
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите **вход с помощью Майкрософт** и во входе с помощью учетной записи глобального администратора Azure AD. После успешного входе вы можете увидеть сведения об учетной записи пользователя в области слева.
    3. Выберите значок параметров справа от сведений учетной записи пользователя, а затем выберите **"Выбор разрешений".**

        ![Выбор разрешений Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. Прокрутите список разрешений для разрешений, разкройте группу `Group` **(2),** выберите разрешение **Group.ReadWrite.All.** Прокрутите список разрешений вниз, разйдите на страницу `User` **User (8)** и выберите разрешение **User.ReadWrite.All.**

        ![Поиск разрешений пользователя, группы и прав на доступ](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. Выберите **"Согласие",** а затем выберите **"Принять",** чтобы принять согласие на разрешения. Для получения этих разрешений не требуется согласие от имени вашей организации.
    6. Найщите разрешения, развящите `EntitlementManagement` **EntitlementManagement (2),** выберите **разрешение Entitlement.ReadWrite.All,** а затем выберите **"Согласие".** Поскольку это разрешение требует согласия администратора и требуется учетной записи пользователя, которую вы создали в этом руководстве, необходимо выбрать "Согласие" от имени **вашей организации.**

        ![Согласие для организации](./images/tutorial-access-package-api/consent-for-organization.png)

    7. Select **Accept** to accept the consent of the permissions.

## <a name="step-1-create-a-user-account-and-a-group"></a>Шаг 1. Создание учетной записи пользователя и группы

На этом этапе создается  группа "Маркетинговые ресурсы" в каталоге, который является целевым ресурсом для управления правами. Также создается учетная запись пользователя, настроенная как внутренний запросчик.

### <a name="create-a-user-account"></a>Создание учетной записи пользователя

В этом руководстве вы создаете учетную запись пользователя, которая используется для запроса доступа к ресурсам в пакете доступа. При этом измените доменное имя `contoso.onmicrosoft.com` клиента. Сведения о клиенте можно найти на странице обзора Azure Active Directory. Зафиксировать значение **свойства id,** которое будет использоваться далее в руководстве.

#### <a name="request"></a>Запрос

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a>Создание группы

В этом руководстве вы создаете группу с именем **"Маркетинговые** ресурсы", которая является целевым ресурсом для управления правами. Можно использовать существующую группу, если она уже существует. Зафиксировать значение **свойства id,** которое будет возвращено для использования далее в этом руководстве. 

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a>Шаг 2. Добавление ресурсов в каталог и создание пакета доступа

Пакет *доступа —* это набор ресурсов, необходимых группе или проекту и управляемых политиками. Пакеты доступа определяются в контейнерах, называемых каталогами. Каталоги могут ссылаться на ресурсы, такие как группы, приложения и сайты, используемые в пакете доступа. На этом этапе создается **пакет** доступа для маркетинговой кампании в общем каталоге. Если у вас другой каталог, используйте его имя в следующем разделе.

### <a name="get-the-catalog-identifier"></a>Получить идентификатор каталога

Чтобы добавить ресурсы в каталог, необходимо сначала получить его идентификатор. Если вы используете общий каталог, запустите следующий запрос, чтобы получить его идентификатор. Если используется другой calalog, измените значение фильтра в запросе на имя каталога. Зафиксировать значение **свойства id,** которое будет возвращено для использования далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

Ответ должен содержать только каталог, имя которого вы предоставили в запросе. Если значения не возвращаются, перед тем как продолжить, убедитесь, что имя каталога правильное.

### <a name="add-the-group-to-the-catalog"></a>Добавление группы в каталог

Чтобы добавить созданную группу в каталог, укайте следующие значения свойств:
- **catalogId** **— ид** используемого каталога
- **displayName** — имя группы
- **description** — описание группы
- **originId** **— ид** созданной группы

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a>Получить ресурсы каталога

Далее в этом руководстве  вам потребуется ид, который был назначен ресурсу группы в каталоге. Этот идентификатор, который представляет группу как ресурс в каталоге, отличается от идентификатора самой группы в Microsoft Graph. Это потому, что у каталога могут быть ресурсы, которые не представлены в Microsoft Graph.

В запросе укадать **ид** используемого каталога. Зафиксировать значение **свойства id** для ресурса каталога групп.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a>Получить роли ресурсов

Пакет доступа назначает пользователям роли ресурса. Типичная роль группы — это роль участника. Другие ресурсы, такие как сайты и приложения SharePoint Online, могут иметь множество ролей. Типичной ролью группы, используемой в пакете доступа, является роль участника. Роль участника потребуется при добавлении роли ресурса в пакет доступа далее в этом руководстве. 

В запросе используйте  ид каталога  и ид ресурса группы в каталоге, записанный для получения **originId** роли ресурса Member. Зафиксировать значение свойства **originId** для использования далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

В случае успеха возвращается одно значение, которое представляет роль участника этой группы. Если роли не возвращаются, проверьте значения **id** каталога и ресурса пакета доступа.

### <a name="create-the-access-package"></a>Создание пакета доступа

На этом этапе у вас есть каталог с ресурсом группы, и вы знаете, что будете использовать роль ресурса участника группы в пакете доступа. Далее необходимо создать пакет доступа. После получения пакета доступа вы можете добавить в него роль ресурса и создать политику, чтобы пользователи могли запрашивать доступ к этой роли ресурса. Для создания пакета доступа используется **ид** каталога, записанный ранее. **Зафиксировать ид** пакета доступа для использования далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a>Добавление роли ресурса в пакет доступа

Добавьте роль "Участник" ресурса группы в пакет доступа. В запросе укадать **ид** пакета доступа. В теле запроса  удайте ид ресурса каталога группы для accessPackageResource и укажийте **originId** роли Member, которую вы ранее записаны.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

Пакет доступа теперь имеет одну роль ресурса, которая является членством в группах. Роль назначена любому пользователю, у которого есть пакет доступа.

### <a name="create-an-access-package-policy"></a>Создание политики пакетов доступа

Теперь, когда вы создали пакет доступа и добавили ресурсы и роли, вы можете решить, кто может получить к нему доступ, создав политику пакета доступа. В этом руководстве вы включаете созданную учетную запись **Requestor1** для запроса доступа к ресурсам в пакете доступа. Для этой задачи необходимы указанные здесь значения.
- **ид** пакета доступа для значения свойства **accessPackageId**
- **ид** **учетной записи пользователя Requestor1** для значения свойства **id** в **allowedRequestors**
 
Значение свойства **durationInDays** позволяет учетной записи **Requestor1** получать доступ к ресурсам в пакете доступа в течение 30 дней. Зафиксировать значение **свойства id,** которое будет возвращено для использования далее в этом руководстве. 

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a>Шаг 3. Запрос доступа

На этом этапе учетная запись **пользователя Requestor1** запрашивает доступ к ресурсам в пакете доступа.

Чтобы запросить доступ к ресурсам в пакете доступа, необходимо предоставить указанные значения.
- **ид** **учетной записи пользователя Requestor1,** созданной для значения **свойства targetId**
- **ид** политики назначения для значения свойства **assignmentPolicyId**
- **ид** пакета доступа для значения свойства **accessPackageId**

В ответе можно увидеть  состояние "Принято" и **"Отправлено".** Зафиксировать значение **свойства id,** возвращаемого для получения состояния запроса позже.

Если вы еще не сделали этого, вы можете выйти из учетной записи администратора, используемой в проводнике Microsoft Graph. Во sign in to the **Requestor1** user account that you created. Вам будет предложено изменить пароль при первом входе.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a>Шаг 4. Проверка того, что доступ назначен

На этом этапе вы подтверждаете, что учетной записи пользователя **Requestor1** назначен пакет доступа и что они теперь являются членами группы **"Маркетинговые ресурсы".**

Вы можете выйти из учетной записи Requestor1 и войти в учетную запись администратора, чтобы увидеть состояние запроса.

### <a name="get-the-status-of-the-request"></a>Получить состояние запроса

Используйте значение свойства **id** запроса, чтобы получить его текущее состояние. В ответе можно увидеть, что состояние изменено на **"Выполнено",** а состояние изменено на **"Доставлено".**

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a>Получить назначения пакетов доступа

Вы также можете использовать **ид** созданной политики пакета доступа, чтобы увидеть, что ресурсы назначены учетной записи пользователя **Requestor1.**

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a>Ответ

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a>Получить участников группы

После предоставления запроса можно использовать ид, записанный для  группы "Маркетинговые ресурсы", чтобы увидеть, что учетная запись пользователя **Requestor1** добавлена в нее. 

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a>Отклик:

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a>Шаг 5. Очистка ресурсов

На этом этапе вы удалите внесенные изменения и удалите пакет доступа **к** маркетинговой кампании.

### <a name="remove-an-access-package-assignment"></a>Удаление назначения пакета доступа

Перед удалением необходимо удалить все назначения пакета доступа. Используйте **ид запроса** на назначение, записанного ранее, чтобы удалить его.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a>Ответ

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a>Удаление политики назначения пакета доступа

Используйте **для удаления ранее** записанную политику назначения. Сначала убедитесь, что все назначения удалены.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-access-package"></a>Удаление пакета доступа

Используйте **ид пакета** доступа, записанного ранее, чтобы удалить его.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите **учетную запись пользователя Requestor1.**

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-group"></a>Добавлять и удалять участников группы.

Удалите **группу маркетинговых** ресурсов.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

## <a name="see-also"></a>См. также

В этом руководстве вы использовали множество API для выполнения задач. Изучите справочник по API для этих API, чтобы узнать больше о том, что могут делать API.


- [Работа с API управления правами Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [accessPackageResourceRoleScope](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [group](/graph/api/resources/group?view=graph-rest-1.0)
- [user](/graph/api/resources/user?view=graph-rest-1.0)