---
title: Руководство. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Graph Майкрософт
description: Узнайте, как управлять доступом к ресурсам в управлении правами Active Directory (Azure AD) с помощью API Graph Майкрософт.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 4a241d09897e51b4395f867351d51f6be9ef1e2d
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366123"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a>Руководство. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Graph Майкрософт

Управление доступом ко всем ресурсам, которые требуются сотрудникам, таким как группы, приложения и сайты, является важной функцией для организаций. Вы хотите предоставить сотрудникам нужный уровень доступа, необходимый для продуктивной работы, и удалить их доступ, когда он больше не нужен. [Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) с помощью API Microsoft Graph позволяет управлять этим типом доступа.

В этом руководстве вам было предложено разработать код для создания пакета ресурсов для маркетинговой кампании, которую внутренние пользователи могут запрашивать самостоятельно. Запросы не требуют утверждения, и срок действия доступа пользователя истекает через 30 дней. В этом руководстве ресурсы маркетинговой кампании — это просто членство в одной группе, но это может быть коллекция групп, приложений или SharePoint веб-сайтов.

>**Примечание:** Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости. 

## <a name="prerequisites"></a>Предварительные требования

Для успешного завершения работы с этим руководством убедитесь, что у вас есть необходимые компоненты:
- Azure AD управления правами требуются определенные лицензии. Дополнительные сведения см [. в разделе "Требования к лицензии"](/azure/active-directory/governance/entitlement-management-overview#license-requirements). В клиенте требуются следующие лицензии:
    - Azure AD Premium P2
    - Enterprise Mobility + Security (EMS) E5
- В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями. Для работы с этим руководством требуются `User.ReadWrite.All``Group.ReadWrite.All``EntitlementManagement.ReadWrite.All` делегированные разрешения и делегированные разрешения. Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD. После успешного входа вы увидите данные учетной записи пользователя на панели слева.
    3. Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.

        ![Выбор разрешений Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. Прокрутите `Group` список разрешений до разрешений, разверните группу **(2)** и выберите разрешение **Group.ReadWrite.All** . Прокрутите `User` список разрешений вниз, разверните узел **User (8)** и выберите разрешение **User.ReadWrite.All** .

        ![Поиск разрешений пользователя, группы и управления правами](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно предоставлять согласие от имени организации для этих разрешений.
    6. Найдите разрешения `EntitlementManagement` , разверните **EntitlementManagement (2),** выберите разрешение **Entitlement.ReadWrite.All** , а затем выберите **"Согласие"**. Так как это разрешение требует согласия администратора и требуется учетной записи пользователя, которую вы создаете в этом руководстве, необходимо выбрать согласие от **имени организации**.

        ![Согласие для организации](./images/tutorial-access-package-api/consent-for-organization.png)

    7. Выберите **"Принять** ", чтобы принять согласие на разрешения.

## <a name="step-1-create-a-user-account-and-a-group"></a>Шаг 1. Создание учетной записи пользователя и группы

На этом шаге вы создайте группу с именем **"** Маркетинговые ресурсы" в каталоге, который является целевым ресурсом для управления правами. Вы также создаете учетную запись пользователя, настроенную в качестве внутреннего инициатора запроса.

### <a name="create-a-user-account"></a>Создание учетной записи пользователя

В этом руководстве создается учетная запись пользователя, которая используется для запроса доступа к ресурсам в пакете доступа. При выполнении этих вызовов измените `contoso.onmicrosoft.com` доменное имя клиента. Информацию о клиенте можно найти на странице обзора в Azure Active Directory. Запишите значение свойства **идентификатора** , которое будет использоваться далее в этом руководстве.

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

#### <a name="response"></a>Отклик

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

В этом руководстве вы создайте группу с именем **"Маркетинговые** ресурсы", которая является целевым ресурсом для управления правами. Вы можете использовать существующую группу, если она у вас уже есть. Запишите значение свойства **идентификатора** , которое будет использоваться далее в этом руководстве. 

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

#### <a name="response"></a>Отклик

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

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a>Шаг 2. Добавление ресурсов в каталог и создание пакета для доступа

Пакет *для доступа —* это набор ресурсов, необходимых команде или проекту и управляемых политиками. Пакеты доступа определяются в контейнерах, называемых каталогами. Каталоги могут ссылаться на ресурсы, такие как группы, приложения и сайты, которые используются в пакете доступа. На этом шаге вы создайте **пакет доступа** маркетинговой кампании в каталоге "Общие". Если у вас другой каталог, используйте его имя в следующем разделе.

### <a name="get-the-catalog-identifier"></a>Получение идентификатора каталога

Чтобы добавить ресурсы в каталог, необходимо сначала получить его идентификатор. Если вы используете общий каталог, выполните следующий запрос, чтобы получить его идентификатор. Если вы используете другой calalog, измените значение фильтра в запросе на имя каталога. Запишите значение свойства **идентификатора** , которое будет использоваться далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a>Отклик

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

Ответ должен содержать только каталог, имя которого вы указали в запросе. Если значения не возвращаются, перед продолжением убедитесь, что имя каталога правильное.

### <a name="add-the-group-to-the-catalog"></a>Добавление группы в каталог

Чтобы добавить группу, созданную в каталоге, укажите следующие значения свойств:
- **catalogId** — **идентификатор** каталога, который вы используете
- **displayName** — имя группы
- **description** — описание группы
- **originId** — **идентификатор** созданной группы

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

#### <a name="response"></a>Отклик

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

### <a name="get-catalog-resources"></a>Получение ресурсов каталога

Далее в этом руководстве вам потребуется идентификатор,  назначенный ресурсу группы в каталоге. Этот идентификатор, представляющий группу в качестве ресурса в каталоге, отличается от идентификатора самой группы в Microsoft Graph. Это связано с тем, что каталог может содержать ресурсы, которые не представлены в microsoft Graph.

В запросе укажите **идентификатор** каталога, который вы используете. Запишите значение свойства **идентификатора** для ресурса каталога групп.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a>Отклик

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

### <a name="get-resources-roles"></a>Получение ролей ресурсов

Пакет доступа назначает пользователям роли ресурса. Типичной ролью группы является роль участника. Другие ресурсы, такие как SharePoint веб-сайтов и приложений, могут иметь множество ролей. Типичной ролью группы, используемой в пакете доступа, является роль участника. Роль участника потребуется при добавлении роли ресурса в пакет для доступа далее в этом руководстве. 

В запросе используйте идентификатор каталога и идентификатор ресурса группы в каталоге, который вы записали, чтобы получить **originId** роли ресурса-члена.  Запишите значение свойства **originId** , которое будет использоваться далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a>Отклик

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
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

В случае успешного выполнения возвращается одно значение, представляющее роль участника этой группы. Если роли не возвращаются, проверьте значения **идентификаторов** каталога и ресурса пакета доступа.

### <a name="create-the-access-package"></a>Создание пакета для доступа

На этом этапе у вас есть каталог с ресурсом группы, и вы знаете, что будете использовать роль ресурса члена группы в пакете доступа. Следующим шагом является создание пакета доступа. Получив пакет доступа, вы можете добавить в него роль ресурса и создать политику, чтобы пользователи могли запрашивать доступ к этой роли ресурса. Для создания **пакета доступа** используется идентификатор каталога, записанного ранее. Запишите **идентификатор пакета** для доступа, который будет использоваться далее в этом руководстве.

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

#### <a name="response"></a>Отклик

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

### <a name="add-a-resource-role-to-the-access-package"></a>Добавление роли ресурса в пакет для доступа

Добавьте роль участника ресурса группы в пакет доступа. В запросе укажите **идентификатор** пакета доступа. В тексте запроса укажите идентификатор ресурса каталога группы для accessPackageResource и укажите идентификатор источника  роли участника, записанной ранее.

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

#### <a name="response"></a>Отклик

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

Пакет доступа теперь имеет одну роль ресурса, то есть членство в группе. Роль назначается любому пользователю, у которого есть пакет доступа.

### <a name="create-an-access-package-policy"></a>Создание политики пакетов для доступа

Теперь, когда вы создали пакет доступа и добавили ресурсы и роли, вы можете решить, кто может получить к нему доступ, создав политику пакетов доступа. В этом руководстве описано, как включить созданную учетную запись **Requestor1** для запроса доступа к ресурсам в пакете доступа. Для этой задачи вам потребуются следующие значения:
- **Идентификатор пакета** доступа для значения свойства **accessPackageId**
- **Идентификатор учетной** **записи пользователя Requestor1** для значения свойства **идентификатора** в **allowedRequestors**
 
Значение свойства **durationInDays** позволяет учетной записи **Requestor1** получать доступ к ресурсам в пакете доступа на срок до 30 дней. Запишите значение свойства **идентификатора** , которое будет использоваться далее в этом руководстве. 

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

#### <a name="response"></a>Отклик

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

На этом шаге **учетная запись пользователя Requestor1** запрашивает доступ к ресурсам в пакете доступа.

Чтобы запросить доступ к ресурсам в пакете для доступа, необходимо указать следующие значения:
- **Идентификатор учетной** **записи пользователя Requestor1**, созданной для значения свойства **targetId**
- **Идентификатор политики** назначения для значения свойства **assignmentPolicyId**
- **Идентификатор пакета** доступа для значения свойства **accessPackageId**

В ответе можно увидеть состояние **"Принято** " и " **Отправлено"**. Запишите значение свойства **идентификатора** , которое возвращается для получения состояния запроса позже.

Если вы еще не сделали этого, выйдите из учетной записи администратора, которую вы использовали в Microsoft Graph Explorer. Войдите в **созданную учетную запись пользователя Requestor1** . При первом входе вам будет предложено изменить пароль.

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

#### <a name="response"></a>Отклик

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

## <a name="step-4-validate-that-access-has-been-assigned"></a>Шаг 4. Проверка назначения доступа

На этом шаге вы подтверждаете, что учетной записи **пользователя Requestor1** был назначен пакет доступа и что они теперь являются участником группы **маркетинговых** ресурсов.

Выйдите из учетной записи Requestor1 и войдите в учетную запись администратора, чтобы просмотреть состояние запроса.

### <a name="get-the-status-of-the-request"></a>Получение состояния запроса

Используйте значение свойства **идентификатора** запроса, чтобы получить его текущее состояние. В ответе можно увидеть, что состояние изменилось на **"** Выполнено", а состояние — на **"Доставлено"**.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a>Отклик

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

### <a name="get-access-package-assignments"></a>Получение назначений пакетов для доступа

Вы также можете использовать **идентификатор** созданной политики пакетов доступа, чтобы увидеть, что ресурсы были назначены учетной записи **пользователя Requestor1** .

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'&$expand=target,accessPackageAssignmentResourceRoles
```

#### <a name="response"></a>Отклик

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
      "expiredDateTime": null,
      "target": {
         "id": "8586ddc8-0ff7-4c24-9c79-f192bc3566e3",
         "objectId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0"
      },
      "accessPackageAssignmentResourceRoles": [
         {
            "id": "bdb7e0a0-a927-42ab-bf30-c5b5533dc54a",
            "originSystem": "AadGroup",
            "status": "Fulfilled"
         }
      ]
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a>Получение участников группы

После предоставления запроса можно использовать идентификатор, записанный для группы  маркетинговых ресурсов, чтобы увидеть, что  к ней добавлена учетная запись пользователя **Requestor1**.

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

На этом шаге вы удалите внесенные изменения и удалите пакет доступа **маркетинговой** кампании.

### <a name="remove-an-access-package-assignment"></a>Удаление назначения пакета для доступа

Перед удалением необходимо удалить все назначения пакета доступа. Используйте **идентификатор запроса** на назначение, записанного ранее, чтобы удалить его.

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

#### <a name="response"></a>Отклик

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

### <a name="delete-the-access-package-assignment-policy"></a>Удаление политики назначения пакетов для доступа

Используйте **идентификатор политики** назначения, записанной ранее, чтобы удалить ее. Сначала убедитесь, что все назначения удалены.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-access-package"></a>Удаление пакета для доступа

Используйте **идентификатор пакета** доступа, который вы записали ранее, чтобы удалить его.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите **учетную запись пользователя Requestor1** .

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-group"></a>Добавлять и удалять участников группы.

Удалите **группу маркетинговых** ресурсов.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

## <a name="see-also"></a>См. также

В этом руководстве вы использовали множество API для выполнения задач. Дополнительные сведения о возможностях API см. в справочнике по API для этих API.


- [Работа с API Azure AD управления правами](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true)
- [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
- [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
- [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
- [accessPackageResourceRoleScope](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta&preserve-view=true)
- [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
- [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
- [group](/graph/api/resources/group)
- [user](/graph/api/resources/user?)
