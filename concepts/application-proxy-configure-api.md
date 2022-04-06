---
title: Настройка Application Proxy с помощью API Graph Майкрософт
description: Настройте Application Proxy API Microsoft Graph для предоставления удаленного доступа и единого входа в локальные приложения.
author: davidmu1
ms.topic: conceptual
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: c6466de02e1521889db27b509bc0ecb2d07cd4af
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685210"
---
# <a name="configure-application-proxy-using-the-microsoft-graph-api"></a>Настройка Application Proxy с помощью microsoft API Graph

Из этой статьи вы узнаете, как настроить Azure Active Directory (Azure AD) Application Proxy для приложения. Application Proxy обеспечивает безопасный удаленный доступ и единый вход в локальные веб-приложения. После настройки Application Proxy приложения пользователи могут получить доступ к локальным приложениям через внешний URL-адрес, портал Мои приложения или другие внутренние порталы приложений.

## <a name="prerequisites"></a>Предварительные условия

- В этом руководстве предполагается, что вы уже установили соединитель и [](/azure/active-directory/app-proxy/application-proxy-add-on-premises-application#prerequisites) выполнили необходимые условия для Application Proxy, чтобы соединители могли взаимодействовать со службами Azure AD.
- В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями. Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD. После успешного входа вы увидите данные учетной записи пользователя на панели слева.
    3. Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.

        ![Установка разрешений](./images/application-proxy-configure-api/set-permissions.png)
        
    4. Прокрутите список разрешений для **каталога (3),** разверните и выберите .`Directory.ReadWrite.All`

        ![Поиск разрешений](./images/application-proxy-configure-api/select-permissions.png)
    
    5. Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно предоставлять согласие от имени организации для этих разрешений.

        ![Принятие запроса на разрешения](./images/application-proxy-configure-api/accept-permissions.png)

> [!NOTE]
> Отображаемые объекты ответа могут быть сокращены для удобочитаемости. 

## <a name="step-1-create-a-custom-application"></a>Шаг 1. Создание пользовательского приложения

Чтобы настроить Application Proxy для приложения с помощью API, сначала создайте пользовательское приложение, а затем обновите свойство **onPremisesPublishing** приложения, чтобы настроить параметры прокси приложения. В этом руководстве вы используете шаблон приложения для создания экземпляра пользовательского приложения и субъекта-службы в клиенте для управления. The template ID for a custom application is `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

Запишите **идентификатор**, **appId**, **servicePrincipalId** приложения, который будет использоваться далее в этом руководстве.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

## <a name="step-2-configure-application-proxy"></a>Шаг 2. Настройка Application Proxy

Используйте **идентификатор,** записанный для приложения, чтобы начать настройку Application Proxy. Обновите следующие свойства:

- **onPremisesPublishing** . В этом примере вы используете приложение с внутренним URL-адресом: `https://contosoiwaapp.com`. Вы также используете домен по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net`. 
- **redirectUri**, **identifierUri** и **homepageUrl** — задайте тот же внешний URL-адрес, настроенный в свойстве **onPremisesPublishing** .
- **implicitGrantSettings** — задайте для `true` **enabledTokenIssuance** `false` и **enabledAccessTokenIssuance**.

#### <a name="request"></a>Запрос

```http
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: application/json

{
  "onPremisesPublishing": {
    "externalAuthenticationType": "aadPreAuthentication",
    "internalUrl": "https://contosoiwaapp.com",
    "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
  }
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-a-connector-group-to-the-application"></a>Шаг 3. Назначение группы соединителей приложению

### <a name="get-connectors"></a>Получение соединителей

Список доступных соединителей. Запишите **идентификатор соединителя** , который необходимо назначить группе соединителей.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
  "value": [
    {
      "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
      "machineName": "connectorA.redmond.contoso.com"",
      "externalIp": "131.137.147.164",
      "status": "active"
    },
    {
      "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
      "machineName": "connectorB.contoso.com"",
      "externalIp": "68.0.191.210",
      "status": "active"
    }
  ]
}
```

### <a name="create-a-connectorgroup"></a>Создание connectorGroup

В этом примере создается группа соединителей `IWA Demo Connector Group` с именем, которая используется для приложения. Запишите **идентификатор,** который будет возвращен для использования на следующем шаге.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
  "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "IWA Demo Connector Group",
  "connectorGroupType": "applicationProxy",
  "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a>Назначение соединителя для connectorGroup

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/f2cab422-a1c8-4d70-a47e-2cb297a2e051/memberOf/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a>Назначение приложения для connectorGroup

#### <a name="request"></a>Запрос

```http
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a>Шаг 4. Настройка единого входа

Это приложение использует встроенную Windows проверку подлинности (IWA). Чтобы настроить IWA, задайте свойства единого входа для **onPremisesPublishing**.

#### <a name="request"></a>Запрос

```http
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "onPremisesPublishing": {
    "singleSignOnSettings": {
      "kerberosSignOnSettings": {
        "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
      },
      "singleSignOnMode": "onPremisesKerberos"
    }
  } 
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-a-user"></a>Шаг 5. Назначение пользователя

### <a name="retrieve-the-approle-for-the-application"></a>Получение appRole для приложения

Получите роли приложения, используя **идентификатор** субъекта-службы. Запишите **идентификатор роли** приложения **"** Пользователь", которая будет использоваться на следующем шаге.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 200
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
  "value": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "User",
      "displayName": "User",
      "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
      "isEnabled": true,
      "origin": "Application",
      "value": null
    },
  ]
}
```

### <a name="create-a-user-account"></a>Создание учетной записи пользователя

В этом руководстве вы создадим учетную запись пользователя, назначенную роли приложения. В тексте запроса измените `contoso.com` доменное имя клиента. Информацию о клиенте можно найти на странице обзора в Azure Active Directory. Запишите **идентификатор учетной** записи пользователя, которая будет использоваться на следующем шаге.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
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
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

### <a name="assign-the-user-to-the-application"></a>Назначение пользователя приложению

В следующем примере замените значения этих свойств:

- **principalId** с **идентификатором** пользователя
- **appRoleId** с **идентификатором** роли приложения
- **идентификатор ресурса** с **идентификатором** субъекта-службы;

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 200
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
  "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
  "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
  "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "principalDisplayName": "MyTestUser1",
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "resourceDisplayName": "Contoso IWA App",
  "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```
## <a name="step-6-test-access-to-the-application"></a>Шаг 6. Проверка доступа к приложению

Протестируйте приложение, посетив внешний **URL-адрес** , настроенный для приложения в браузере, а затем войдите с помощью тестового пользователя. Вы должны иметь возможность войти в приложение и получить доступ к приложению.

## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Ресурсы, созданные в этом руководстве, не предназначены для использования в рабочей среде. На этом шаге вы удаляете созданные ресурсы.

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите учетную запись пользователя MyTestUser1.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-application"></a>Удаление приложения

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-connector-group"></a>Удаление группы соединителей

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

## <a name="see-also"></a>См. также

- [Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy)
- [application](/graph/api/resources/application?view=graph-rest-1.0)
- [applicationTemplate: создание экземпляра](/graph/api/applicationtemplate-instantiate?view=graph-rest-1.0)
- [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta)
- [connector](/graph/api/resources/connector?view=graph-rest-beta)
- [connectorGroup](/graph/api/resources/connectorGroup?view=graph-rest-beta)
- [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0)
- [локальные профили публикации](/graph/api/resources/onpremisespublishingprofile-root?view=graph-rest-beta)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)
- [user](/graph/api/resources/user?view=graph-rest-1.0)
