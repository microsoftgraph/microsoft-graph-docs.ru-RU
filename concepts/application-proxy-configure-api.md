---
title: Настройка прокси-сервера приложений с Graph API Майкрософт
description: Настройка прокси-приложения с Graph API Майкрософт для обеспечения удаленного доступа и единой входной записи в локальном приложении.
author: davidmu1
ms.topic: conceptual
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 96a1f390b41f585d530b04a831a2d9a79a12aa88
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142427"
---
# <a name="configure-application-proxy-using-the-microsoft-graph-api"></a>Настройка прокси-приложения с помощью API Graph Microsoft

В этой статье вы узнаете, как настроить прокси Azure Active Directory приложения (Azure AD). Прокси-сервер приложения обеспечивает безопасный удаленный доступ и один вход в локальное веб-приложение. После настройки прокси-сервера приложений для приложения пользователи могут получать доступ к своим внутренним приложениям с помощью внешнего URL-адреса, портала "Мои приложения" или других внутренних порталов приложений.

## <a name="prerequisites"></a>Предварительные условия

- В этом руководстве предполагается, что вы [](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) уже установили соединители и выполнили необходимые условия для прокси-сервера приложений, чтобы соединители могли взаимодействовать с службами Azure AD.
- В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями. Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD. После успешного входа вы увидите данные учетной записи пользователя на панели слева.
    3. Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.

        ![Установка разрешений](./images/application-proxy-configure-api/set-permissions.png)
        
    4. Прокрутите список разрешений **в Каталог (3),** разйдите и выберите `Directory.ReadWrite.All` .

        ![Поиск разрешений](./images/application-proxy-configure-api/select-permissions.png)
    
    5. Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно предоставлять согласие от имени организации для этих разрешений.

        ![Прием разрешений](./images/application-proxy-configure-api/accept-permissions.png)

> [!NOTE]
> Показанные объекты отклика могут быть сокращены для читаемости. 

## <a name="step-1-create-a-custom-application"></a>Шаг 1. Создание настраиваемой программы

Чтобы настроить прокси-сервер приложения для приложения с помощью API, сначала создайте настраиваемое приложение, а затем обновим свойство **приложения onPremisesPublishing** для настройки параметров прокси-сервера приложения. В этом руководстве используется шаблон приложения для создания экземпляра настраиваемого приложения и основного клиента для управления. ID шаблона для настраиваемой заявки `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .

Запись **id,** **appId**, **servicePrincipalId** приложения для использования позже в учебнике.

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

## <a name="step-2-configure-application-proxy"></a>Шаг 2. Настройка прокси-сервера приложения

Чтобы запустить конфигурацию прокси-приложения, используйте **id,** записанный для приложения. Обновление следующих свойств:

- **onPremisesPublishing** . В этом примере вы используете приложение с внутренним URL-адресом: `https://contosoiwaapp.com` . Вы также используете домен по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` . 
- **redirectUri,** **identifierUri** и **homepageUrl** — установите тот же внешний URL-адрес, настроенный в **свойстве onPremisesPublishing.**
- **implicitGrantSettings** - Set to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance.**

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

## <a name="step-3-assign-a-connector-group-to-the-application"></a>Шаг 3. Назначение группы соединители для приложения

### <a name="get-connectors"></a>Получить соединители

Список доступных соединитений. **Записываю id** соединитетеля, который необходимо назначить группе соединители.

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

### <a name="create-a-connectorgroup"></a>Создание соединителиГруп

В этом примере создается новый соединитекторGroup, `IWA Demo Connector Group` который используется для приложения. Запись **возвращенного для** использования id на следующем шаге.

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

### <a name="assign-a-connector-to-the-connectorgroup"></a>Назначение соединитетеля соединитетелем connectorGroup

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

### <a name="assign-the-application-to-the-connectorgroup"></a>Назначение приложения в connectorGroup

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

## <a name="step-4-configure-single-sign-on"></a>Шаг 4. Настройка единого входного

Это приложение использует интегрированную Windows проверку подлинности (IWA). Чтобы настроить IWA, установите свойства единого входного знака **для onPremisesPublishing**.

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

Получение ролей приложения для приложения с помощью **id** директора службы. Запись **id** роли **приложения пользователя,** которая будет использоваться на следующем шаге.

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

В этом руководстве создается учетная запись пользователя, назначенная роли приложения. В теле запроса `contoso.com` измените доменное имя клиента. Информацию о клиенте можно найти на странице обзора в Azure Active Directory. Запись **id** учетной записи пользователя, которая будет использоваться на следующем шаге.

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

- **principalId** с **id** пользователя
- **appRoleId** с **id** роли приложения
- **resourceId** с **id** директора службы

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
## <a name="step-6-test-access-to-the-application"></a>Шаг 6. Тестовый доступ к приложению

Проверьте приложение, посетив внешний **URL-адрес,** настроенный для приложения в браузере, а затем во входе с тестируемым пользователем. Вы должны иметь возможность войти в приложение и получить доступ к приложению.

## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

Созданные в этом руководстве ресурсы не предназначены для использования в производственной среде. На этом шаге вы удаляете созданные ресурсы.

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

### <a name="delete-the-connector-group"></a>Удаление группы соединители

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

## <a name="see-also"></a>См. также

- [Прокси-сервер приложения](/azure/active-directory/manage-apps/what-is-application-proxy)
- [application](/graph/api/resources/application?view=graph-rest-1.0)
- [applicationTemplate: instantiate](/graph/api/applicationtemplate-instantiate?view=graph-rest-1.0)
- [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta)
- [connector](/graph/api/resources/connector?view=graph-rest-beta)
- [connectorGroup](/graph/api/resources/connectorGroup?view=graph-rest-beta)
- [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0)
- [локальной публикации профилей](/graph/api/resources/onpremisespublishingprofile-root?view=graph-rest-beta)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)
- [user](/graph/api/resources/user?view=graph-rest-1.0)
