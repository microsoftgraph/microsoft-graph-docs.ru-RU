---
title: 'applicationTemplate: создание экземпляра'
description: Добавьте экземпляр приложения из коллекции приложений Azure AD в каталог.
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 83fa2386e3e083dd515bf8e53f7afe0ada97061c
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059920"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate: создание экземпляра

Пространство имен: microsoft.graph

Добавьте экземпляр приложения из коллекции приложений Azure AD в каталог. Этот API также можно использовать для создания экземпляров приложений, отличных [от коллекции](/azure/active-directory/manage-apps/add-non-gallery-app). Используйте следующий идентификатор для **объекта applicationTemplate** : `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)        |
| :------------------------------------- | :------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Application.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                     |
| Для приложений                            | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{applicationTemplate-id}/instantiate
```

Для создания экземпляров приложений, отличных от коллекции, используйте `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` для `{applicationTemplate-id}`.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
| :------------ | :------------ |
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр   | Тип   | Описание                    |
| :---------- | :----- | :----------------------------- |
| displayName | String | Пользовательское имя приложения |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и новый [объект applicationServicePrincipal](../resources/applicationserviceprincipal.md) в теле отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/229946b9-a9fb-45b8-9531-efa47453ac9e/instantiate
Content-type: application/json

{
    "displayName": "Azure AD SAML Toolkit"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/applicationtemplate-instantiate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/applicationtemplate-instantiate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "id": "20845737-a145-446f-aa3c-77d432903957",
        "appId": "3c653ec4-4e4c-4820-8127-49e3889cad99",
        "applicationTemplateId": "229946b9-a9fb-45b8-9531-efa47453ac9e",
        "createdDateTime": "2022-04-25T16:48:24Z",
        "deletedDateTime": null,
        "displayName": "Azure AD SAML Toolkit",
        "groupMembershipClaims": null,
        "identifierUris": [],
        "isFallbackPublicClient": false,
        "signInAudience": "AzureADMyOrg",
        "tags": [],
        "tokenEncryptionKeyId": null,
        "defaultRedirectUri": null,
        "optionalClaims": null,
        "addIns": [],
        "api": {
            "acceptMappedClaims": null,
            "knownClientApplications": [],
            "requestedAccessTokenVersion": null,
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allow the application to access Azure AD SAML Toolkit on behalf of the signed-in user.",
                    "adminConsentDisplayName": "Access Azure AD SAML Toolkit",
                    "id": "00e7ef81-4deb-41d7-9ee3-90d4eba1e991",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allow the application to access Azure AD SAML Toolkit on your behalf.",
                    "userConsentDisplayName": "Access Azure AD SAML Toolkit",
                    "value": "user_impersonation"
                }
            ],
            "preAuthorizedApplications": []
        },
        "appRoles": [
            {
                "allowedMemberTypes": [
                    "User"
                ],
                "displayName": "msiam_access",
                "id": "8b292bda-39b6-4b77-849e-887565235bb0",
                "isEnabled": true,
                "description": "msiam_access",
                "value": null,
                "origin": "Application"
            }
        ],
        "info": {
            "logoUrl": null,
            "marketingUrl": null,
            "privacyStatementUrl": null,
            "supportUrl": null,
            "termsOfServiceUrl": null
        },
        "keyCredentials": [],
        "parentalControlSettings": {
            "countriesBlockedForMinors": [],
            "legalAgeGroupRule": "Allow"
        },
        "passwordCredentials": [],
        "publicClient": {
            "redirectUris": []
        },
        "requiredResourceAccess": [],
        "verifiedPublisher": {
            "displayName": null,
            "verifiedPublisherId": null,
            "addedDateTime": null
        },
        "web": {
            "homePageUrl": "https://samltoolkit.azurewebsites.net/SAML/Consume?metadata=samltoolkit|ISV9.2|primary|z",
            "redirectUris": [
                "https://samltoolkit.azurewebsites.net/SAML/Consume"
            ]
        }
    },
    "servicePrincipal": {
        "id": "912729dd-97ae-4ceb-ade4-07bed3046486",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appId": "3c653ec4-4e4c-4820-8127-49e3889cad99",
        "applicationTemplateId": "229946b9-a9fb-45b8-9531-efa47453ac9e",
        "appDisplayName": "Azure AD SAML Toolkit",
        "alternativeNames": [],
        "appOwnerOrganizationId": "29a4f813-9274-4e1b-858d-0afa98ae66d4",
        "displayName": "Azure AD SAML Toolkit",
        "appRoleAssignmentRequired": true,
        "loginUrl": null,
        "logoutUrl": null,
        "homepage": "https://samltoolkit.azurewebsites.net/SAML/Consume?metadata=samltoolkit|ISV9.2|primary|z",
        "notificationEmailAddresses": [],
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [
            "https://samltoolkit.azurewebsites.net/SAML/Consume"
        ],
        "servicePrincipalNames": [
            "3c653ec4-4e4c-4820-8127-49e3889cad99"
        ],
        "servicePrincipalType": "Application",
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
        "tokenEncryptionKeyId": null,
        "samlSingleSignOnSettings": null,
        "verifiedPublisher": {
            "displayName": null,
            "verifiedPublisherId": null,
            "addedDateTime": null
        },
        "addIns": [],
        "appRoles": [
            {
                "allowedMemberTypes": [
                    "User"
                ],
                "displayName": "msiam_access",
                "id": "8b292bda-39b6-4b77-849e-887565235bb0",
                "isEnabled": true,
                "description": "msiam_access",
                "value": null,
                "origin": "Application"
            }
        ],
        "info": {
            "logoUrl": null,
            "marketingUrl": null,
            "privacyStatementUrl": null,
            "supportUrl": null,
            "termsOfServiceUrl": null
        },
        "keyCredentials": [],
        "oauth2PermissionScopes": [
            {
                "adminConsentDescription": "Allow the application to access Azure AD SAML Toolkit on behalf of the signed-in user.",
                "adminConsentDisplayName": "Access Azure AD SAML Toolkit",
                "id": "00e7ef81-4deb-41d7-9ee3-90d4eba1e991",
                "isEnabled": true,
                "type": "User",
                "userConsentDescription": "Allow the application to access Azure AD SAML Toolkit on your behalf.",
                "userConsentDisplayName": "Access Azure AD SAML Toolkit",
                "value": "user_impersonation"
            }
        ],
        "passwordCredentials": []
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
