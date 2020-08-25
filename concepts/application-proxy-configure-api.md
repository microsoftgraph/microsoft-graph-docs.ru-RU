---
title: Настройка прокси приложения с помощью API Microsoft Graph
description: Автоматическая настройка прокси приложения с помощью API Microsoft Graph для предоставления удаленного доступа и единого входа в локальные приложения.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873106"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a>Автоматизация настройки прокси-сервера приложений с помощью API Microsoft Graph

В этой статье вы узнаете, как создать и настроить [прокси приложения](https://aka.ms/whyappproxy) Azure Active Directory (Azure AD) для приложения. Прокси приложения обеспечивает безопасный удаленный доступ и единый вход в локальные веб-приложения. После настройки прокси приложения для приложения пользователи могут получать доступ к локальным приложениям с помощью внешнего URL-адреса, портала "Мои приложения" или других внутренних порталов приложений.

В этой статье предполагается, что вы уже установили соединитель и выполнили [необходимые условия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) для прокси приложения, чтобы соединители могли общаться со СЛУЖБАМИ Azure AD.

Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.

|Тип ресурса |Метод |
|---------|---------|
|[applications](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [онпремисеспублишинг](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [Создание приложения](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [Обновление приложения](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [Добавление приложения в Коннекторграуп](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[PDIF](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [Получение соединителей](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [Создание connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [Добавление соединителя для connectorGroup](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[Создать servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [Обновление servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [Создание appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> В запросах, показанных в этой статье, используются примеры значений. Их необходимо обновить. Отображаемые объекты ответа также могут быть сокращены для удобочитаемости. 

## <a name="step-1-create-an-application"></a>Шаг 1: создание приложения

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API

1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
2. Выберите **Вход в систему с помощью Microsoft** и войдите с помощью глобального администратора Azure AD или учетных данных администратора приложения.
3. После успешного входа вы увидите сведения об учетной записи пользователя в области слева.

### <a name="create-an-application"></a>Создание приложения

Чтобы настроить прокси приложения для приложения с помощью API, создайте приложение, добавьте субъект-службу в приложение, а затем обновите свойство **онпремисеспублишинг** приложения, чтобы настроить параметры прокси-сервера приложения. При создании приложения задайте для параметра **сигнинаудиенце** приложения значение "азуреадмйорг".

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

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

### <a name="retrieve-the-application-object-id-and-appid"></a>Получение идентификатора и appId объекта Application
Используйте ответ из предыдущего вызова, чтобы получить и сохранить идентификатор объекта приложения и идентификатор приложения.
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a>Создание servicePrincipal для приложения и добавление обязательных тегов
Используйте **AppID** , чтобы создать субъекта службы для приложения. Затем добавьте теги, необходимые для настройки прокси приложения для приложения.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```

#### <a name="response"></a>Ответ
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a>Шаг 2: Настройка свойств прокси приложения

### <a name="set-the-onpremisespublishing-configuration"></a>Настройка конфигурации Онпремисеспублишинг

С помощью идентификатора объекта Application из предыдущего шага Настройте прокси приложения для приложения и обновите свойство **онпремисеспублишинг** до нужной конфигурации. В этом примере используется приложение с внутренним URL-адресом: `https://contosoiwaapp.com` и с использованием домена по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` . 

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a>Завершение настройки приложения
Обновите свойства **redirectUri**, **идентифиерури**и **хомепажеурл** приложения для внешнего ур, настроенного в свойстве **онпремисеспублишинг** . Затем обновите [имплиЦитгрантсеттингс](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) до `true` **енабледтокениссуанце** и `false` для **енабледакцесстокениссуанце**.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
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

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a>Шаг 3: назначение группы соединителей приложению

### <a name="get-connectors"></a>Получение соединителей

Перечислите соединители и используйте ответ для получения и сохранения идентификатора объекта Connector. Идентификатор объекта Connector будет использоваться для назначения соединителя группе соединителей.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

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
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a>Создание Коннекторграуп
В этом примере создается новый Коннекторграуп с именем "Ива Demo Connector Group Connector", который используется для приложения. Кроме того, вы можете пропустить этот шаг, если соединитель уже назначен соответствующему Коннекторграуп. Извлеките и сохраните идентификатор объекта Коннекторграуп, который будет использоваться на следующем шаге.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

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

### <a name="assign-a-connector-to-the-connectorgroup"></a>Назначение соединителя для Коннекторграуп

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a>Назначение приложения для Коннекторграуп

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a>Шаг 4: Настройка единого входа
Это приложение использует встроенную проверку подлинности Windows (ИВА). Чтобы настроить Ива, установите свойства единого входа в тип ресурса [синглесигнонсеттингс](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
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

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a>Шаг 5. Назначение пользователей
### <a name="retrieve-approle-for-the-applicaiton"></a>Получение Аппроле для приложения

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
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
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

Используйте ответ из предыдущего вызова для получения и сохранения идентификатора Аппроле, который будет использоваться для следующего этапа.
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a>Назначение пользователей и групп для приложения

Используйте следующие свойства, чтобы назначить пользователя приложению.

| Свойство  | Описание |Идентификатор  |
|---------|---------|---------|
| principalId | Идентификатор пользователя, который будет назначен приложению | 2fe96d23-5dc6-4f35-8222-0426a8c115c8 |
| principalType | Тип пользователя | Пользователь |
| аппролеид |  Идентификатор роли приложения по умолчанию для приложения | 18d14569-c3bd-439b-9a66-3a2aee01d14f |
| resourceId | Идентификатор servicePrincipal приложения | a8cac399-cde5-4516-a674-819503c61313 |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).


## <a name="additional-steps"></a>Дополнительные действия
- [Автоматизация конфигурации с помощью примеров PowerShell для прокси-сервера приложений](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
