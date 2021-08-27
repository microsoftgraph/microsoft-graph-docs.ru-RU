---
title: Перечисление объектов identityProvider
description: Получите коллекцию ресурсов поставщика удостоверений, настроенных для клиента и полученных из identityProviderBase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 78146fd0f76d6e5c3e3e32e8c23cb622ebfb6d37
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667857"
---
# <a name="list-identityproviders"></a>Перечисление объектов identityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите коллекцию ресурсов поставщика удостоверений, настроенных для клиента и полученных из [identityProviderBase.](../resources/identityproviderbase.md)

Для клиента Azure AD поставщики могут быть [объектами socialIdentityProviders](../resources/socialidentityprovider.md) или [builtinIdentityProviders.](../resources/builtinidentityprovider.md)

Для Azure AD B2C поставщиками могут быть [объекты socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)или [объекты appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешнего поставщика удостоверений
* Администратор потока внешних ID-пользователей

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов socialIdentityProvider](../resources/socialidentityprovider.md)или [builtinIdentityProvider](../resources/builtinidentityprovider.md) в тексте ответа для клиента Azure AD.

Для клиента Azure AD B2C этот метод возвращает код ответа и коллекцию `200 OK` [объектов socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)или [объектов appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-identity-provider-resources-configured-in-an-azure-ad-tenant"></a>Пример 1. Список всех ресурсов поставщика удостоверений, настроенных в клиенте Azure AD

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
   "value":[
      {
         "@odata.type": "microsoft.graph.builtInIdentityProvider",
         "id": "MSASignup-OAUTH",
         "identityProviderType": "MicrosoftAccount",
         "displayName": "MicrosoftAccount"
      },
      {
         "@odata.type": "#microsoft.graph.socialIdentityProvider",
         "id": "Facebook-OAUTH",
         "displayName": "Facebook",
         "identityProviderType": "Facebook",
         "clientId": "test",
         "clientSecret": "******"
      }
   ]
}
```

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a>Пример 2. Список всех **identityProvider,** настроенных в клиенте Azure AD B2C

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-rtt_AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b3476-rdca-4bef-b321-076fde19750b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/sashawho.onmicrosoft.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "name",
                "givenName": "given_name",
                "surname": "family_name",
                "email": "unique_email"
            }
        },
        {
            "@odata.type": "#microsoft.graph.appleManagedIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "developerId": "UBF8T346G9",
            "serviceId": "com.microsoft.aad.b2c.iuyt.client",
            "keyId": "99P6DD87C4",
            "certificateData": "******"
        }
    ]
}

```
