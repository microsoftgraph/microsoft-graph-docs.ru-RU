---
title: 'Руководство: создание пакета Access с помощью API Microsoft Graph'
description: Узнайте, как создать пакет Access и запросить доступ к нему с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c276289b4e71c96386afd7e2502021249025965b
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288842"
---
# <a name="tutorial-create-an-access-package-using-microsoft-graph-apis"></a>Руководство: создание пакета Access с помощью API Microsoft Graph

Управление доступом ко всем ресурсам, необходимым для сотрудников, таких как группы, приложения и сайты, является важной функцией для организаций. Вы хотите предоставить сотрудникам необходимый уровень доступа, который им необходим для продуктивности, и удалить доступ, когда он больше не нужен. [Управление обслуживанием Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) с помощью API Microsoft Graph позволяет управлять этим типом доступа.

В этом руководстве вы запросили разработку кода для создания пакета ресурсов для маркетинговой кампании, с которой внутренние пользователи могут самостоятельно выполнить запрос. Запросы не требуют утверждения и срок действия доступа пользователя истечет через 30 дней. В этом руководстве ресурсы маркетинговой кампании — это всего лишь членство в одной группе, но может быть коллекцией групп, приложений или сайтов SharePoint Online.

>**Примечание:** Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости. 

## <a name="prerequisites"></a>Необходимые компоненты

Для успешного выполнения этого руководства убедитесь, что у вас есть необходимые компоненты:
- Для управления обслуживанием Azure AD требуются определенные лицензии. Более подробную информацию можно узнать в статье [требования к лицензии](/azure/active-directory/governance/entitlement-management-overview#license-requirements). В клиенте требуются следующие лицензии:
    - Azure AD Premium P2
    - Лицензия Enterprise Mobility + Security (EMS)
- В этом руководстве предполагается, что используется обозреватель Microsoft Graph, но вы можете использовать POST или создать собственное клиентское приложение для вызова Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, необходимо использовать учетную запись с ролью глобального администратора и соответствующими разрешениями. В этом руководстве `User.ReadWrite.All` `Group.ReadWrite.All` `EntitlementManagement.ReadWrite.All` необходимы разрешения, и делегированные разрешения. Выполните следующие действия, чтобы задать разрешения в Microsoft Graph Explorer:
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите **Вход в систему с** помощью учетной записи Майкрософт и войдите с помощью учетной записи глобального администратора Azure AD. После успешного входа вы сможете просмотреть сведения об учетной записи пользователя в области слева.
    3. Нажмите значок Параметры справа от сведений учетной записи пользователя, а затем выберите **пункт Выбор разрешений**.

        ![Выбор разрешений Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. Прокрутите список разрешений для `Group` разрешений, разверните **группу (2)**, выберите разрешение **Group. ReadWrite. ALL** . Прокрутите список разрешений на все разрешения `User` , разверните **пользователь (8)** и выберите разрешение **User. ReadWrite. ALL** .

        ![Поиск разрешений "пользователь", "Группа" и "ентитлементманажемент"](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. Выберите **согласие**, а затем нажмите кнопку **принять** , чтобы принять разрешение разрешений. Вы не обязаны согласие от имени вашей организации для этих разрешений.
    6. Выполните поиск `EntitlementManagement` разрешений, разверните **ентитлементманажемент (2)**, выберите разрешения правого доступа **. ReadWrite. ALL** , а затем выберите **согласие**. Так как для этого разрешения требуется согласие администратора и для учетной записи пользователя, созданной в этом руководстве, необходимо выбрать **согласие от имени вашей организации**.

        ![Согласие для Организации](./images/tutorial-access-package-api/consent-for-organization.png)

    7. Нажмите кнопку **принять** , чтобы принять разрешение разрешений.

## <a name="step-1-create-a-user-account-and-a-group"></a>Шаг 1: создание учетной записи пользователя и группы

На этом шаге создается группа с именем " **маркетинговые ресурсы** " в каталоге, который является целевым ресурсом для управления обслуживанием. Вы также создаете учетную запись пользователя, которая настроена как внутренний запрашивающий.

### <a name="create-a-user-account"></a>Создание учетной записи пользователя

В этом руководстве показано, как создать учетную запись пользователя, которая будет использоваться для запроса доступа к ресурсам в пакете Access. При совершении этих вызовов замените `contoso.onmicrosoft.com` доменное имя клиента. Сведения о клиенте можно найти на странице "Обзор Azure Active Directory". Запишите значение свойства **ID** , которое возвращается в дальнейшем для использования в руководстве.

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

В этом руководстве описывается создание группы под названием " **маркетинговые ресурсы** ", которая является целевым ресурсом для управления обслуживанием. Вы можете использовать существующую группу, если она уже есть. Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве. 

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

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a>Шаг 2: Добавление ресурсов в каталог и создание пакета Access

*Пакет Access* — это набор ресурсов, необходимых группе или проекту и управляемых политиками. Пакеты доступа определяются в контейнерах, которые называются каталогами. Каталоги могут ссылаться на ресурсы, такие как группы, приложения и сайты, которые используются в пакете Access. На этом этапе вы создадите пакет доступа к **маркетинговой кампании** в общем каталоге. Если у вас другой каталог, используйте его имя в следующем разделе.

### <a name="get-the-catalog-identifier"></a>Получение идентификатора каталога

Чтобы добавить ресурсы в каталог, необходимо сначала получить его идентификатор. Если вы используете общий каталог, выполните следующий запрос, чтобы получить идентификатор. Если вы используете другой калалог, измените значение фильтра в запросе на имя каталога. Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве.

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

Ответ должен содержать только каталог, имя которого указано в запросе. Если значения не возвращены, проверьте правильность имени каталога, прежде чем продолжить.

### <a name="add-the-group-to-the-catalog"></a>Добавление группы в каталог

Чтобы добавить группу, созданную для каталога, укажите следующие значения свойств:
- **каталогид** — **идентификатор** каталога, который вы используете
- **DisplayName** — имя группы.
- **Description** — описание группы.
- **оригинид** — **идентификатор** созданной группы.

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

Дальнейшие действия, описанные в этом руководстве, потребуют **идентификатор** , назначенный ресурсу группы в каталоге. Этот идентификатор, который представляет группу как ресурс в каталоге, отличается от идентификатора самой группы в Microsoft Graph. Это связано с тем, что каталог может иметь ресурсы, которые не представлены в Microsoft Graph.

В запросе укажите **идентификатор** каталога, который вы используете. Запишите значение свойства **ID** для ресурса каталога группы.

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

Пакет Access назначает пользователей ролям ресурса. Типичной ролью группы является роль участника. Другие ресурсы, например сайты и приложения SharePoint Online, могут иметь множество ролей. Типичной ролью группы, используемой в пакете Access, является роль участника. Роль участника потребуется при добавлении роли ресурса в пакет Access позже в этом руководстве. 

В запросе используйте **идентификатор** каталога и **идентификатор** ресурса Group в каталоге, который вы записали, чтобы получить **оригинид** роли ресурса члена. Запишите значение свойства **оригинид** , которое будет использоваться далее в этом руководстве.

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

В случае успешного выполнения возвращается одно значение, представляющее роль участника для этой группы. Если роли не возвращаются, проверьте значения **ID** каталога и ресурса пакета Access.

### <a name="create-the-access-package"></a>Создание пакета Access

На этом шаге у вас есть каталог с ресурсом Group, и вы знаете, что вы используете роль ресурса "член группы" в пакете Access. Следующий шаг — создание пакета Access. После получения пакета Access можно добавить в него роль ресурса и создать политику, определяющую, как пользователи могут запрашивать доступ к этой роли ресурса. Для создания пакета доступа используется **идентификатор** каталога, записанный ранее. Запишите **идентификатор** пакета доступа, который будет использоваться далее в этом руководстве.

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

### <a name="add-a-resource-role-to-the-access-package"></a>Добавление роли ресурса в пакет Access

Добавьте роль участника для ресурса Group в пакет Access. В запросе укажите **идентификатор** пакета Access. В тексте запроса укажите **идентификатор** ресурса каталога группы для акцесспаккажересаурце и предоставьте **оригинид** роли члена, который вы ранее записали.

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

Пакет Access теперь имеет одну роль ресурса, которая является членством в группе. Роль назначается любому пользователю с пакетом доступа.

### <a name="create-an-access-package-policy"></a>Создание политики пакетов Access

Теперь, когда вы создали пакет Access и добавили ресурсы и роли, вы можете определить, кто может получить доступ к нему, создав политику пакетов Access. В этом руководстве показано, как включить созданную учетную запись **Requestor1** для запроса доступа к ресурсам в пакете Access. Для выполнения этой задачи необходимы следующие значения:
- **идентификатор** пакета доступа для значения свойства **акцесспаккажеид**
- **идентификатор** учетной записи пользователя **Requestor1** для значения свойства **ID** в **алловедрекуесторс**
 
Значение свойства **дуратиониндайс** позволяет учетной записи **Requestor1** получать доступ к ресурсам в пакете Access в течение 30 дней. Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве. 

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

## <a name="step-3-request-access"></a>Шаг 3: запрос доступа

На этом этапе учетная запись пользователя **Requestor1** запрашивает доступ к ресурсам в пакете Access.

Чтобы запросить доступ к ресурсам в пакете Access, необходимо указать следующие значения:
- **идентификатор** учетной записи пользователя **Requestor1** , созданной для значения свойства **targetId**
- **идентификатор** политики назначения для значения свойства **ассигнментполициид**
- **идентификатор** пакета доступа для значения свойства **акцесспаккажеид**

В ответ вы можете просмотреть состояние **принятого** и **отправленного**сообщения. Запишите значение свойства **ID** , которое возвращается для получения состояния запроса позже.

Если вы еще не сделали этого, выйдите из учетной записи администратора, которая использовалась в обозревателе Microsoft Graph. Войдите в созданную учетную запись пользователя **Requestor1** . Вам будет предложено сменить пароль, если вы первый раз входите в нее.

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

## <a name="step-4-validate-that-access-has-been-assigned"></a>Шаг 4: Проверка назначения доступа

На этом этапе вы подтверждаете, что учетной записи пользователя **Requestor1** был назначен пакет доступа и он теперь является участником группы " **маркетинговые ресурсы** ".

Выйдите из учетной записи Requestor1 и войдите в учетную запись администратора, чтобы увидеть состояние запроса.

### <a name="get-the-status-of-the-request"></a>Получение состояния запроса

Используйте значение свойства **ID** запроса для получения текущего состояния. В ответе вы можете увидеть состояние "выполнено", а состояние " **выполнено** " изменено на " **доставлено**".

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

### <a name="get-access-package-assignments"></a>Назначения для получения пакетов Access

Вы также можете использовать **идентификатор** созданной вами политики пакета Access, чтобы увидеть, что для учетной записи пользователя **Requestor1** назначены ресурсы.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
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
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a>Получение членов группы

После предоставления запроса вы можете использовать **идентификатор** , записанный для группы " **маркетинговые ресурсы** ", чтобы убедиться в том, что в нее добавлена учетная запись пользователя **Requestor1** .

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

## <a name="step-5-clean-up-resources"></a>Шаг 5: Очистка ресурсов

На этом шаге вы удаляете внесенные вами изменения и удаляете пакет доступа к **маркетинговой кампании** .

### <a name="remove-an-access-package-assignment"></a>Удаление назначения пакета Access

Перед удалением пакета Access необходимо удалить из него все назначения. Используйте **идентификатор** запроса на назначение, который вы ранее записали, чтобы удалить его.

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

### <a name="delete-the-access-package-assignment-policy"></a>Удаление политики назначения пакетов Access

Используйте **идентификатор** ранее записанной политики назначения, чтобы удалить его. Убедитесь, что сначала удаляются все назначения.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-access-package"></a>Удаление пакета Access

Используйте **идентификатор** пакета Access, который вы ранее записали, чтобы удалить его.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите учетную запись пользователя **Requestor1** .

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-group"></a>Добавлять и удалять участников группы.

Удаление группы **маркетинговых ресурсов** .

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

## <a name="see-also"></a>См. также

В этом руководстве показано, как использовать многие API для выполнения задач. Изучите Справочник по API для этих API, чтобы узнать больше о возможных действиях API.


- [Работа с API управления обслуживанием Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [акцесспаккажекаталог](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [акцесспаккажересаурцерекуест](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [акцесспаккаже](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [акцесспаккажересаурцеролескопе](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [акцесспаккажеассигнментполици](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [акцесспаккажеассигнментрекуест](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [group](/graph/api/resources/group?view=graph-rest-1.0)
- [user](/graph/api/resources/user?view=graph-rest-1.0)