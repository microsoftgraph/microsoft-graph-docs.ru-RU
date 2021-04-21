---
title: Перечисление объектов identityProvider
description: Извлечение списка объектов identityProviderbase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 47e136bc63cd7b95bdcf3778047eb77db58c8de0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921388"
---
# <a name="list-identityproviders"></a><span data-ttu-id="afedf-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="afedf-103">List identityProviders</span></span>
<span data-ttu-id="afedf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afedf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afedf-105">Извлечение списка коллекции объектов, унаследованных от [identityProviderBase.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="afedf-105">Retrieve a list of collection of object inherited from  [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="afedf-106">Для клиента Azure AD это могут быть [объекты socialIdentityProviders](../resources/socialidentityprovider.md) и/или [builtinIdentityProviders.](../resources/builtinidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="afedf-106">For an Azure AD tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md) and/or [builtinIdentityProviders](../resources/builtinidentityprovider.md) objects.</span></span>

<span data-ttu-id="afedf-107">Для клиента Azure AD B2C это могут быть объекты [socialIdentityProviders,](../resources/socialidentityprovider.md) [openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) и/или [объекты appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="afedf-107">For an Azure AD B2C tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="afedf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afedf-108">Permissions</span></span>

<span data-ttu-id="afedf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afedf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afedf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afedf-111">Permission type</span></span>      | <span data-ttu-id="afedf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afedf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afedf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afedf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afedf-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afedf-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="afedf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afedf-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="afedf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afedf-116">Not supported.</span></span>|
|<span data-ttu-id="afedf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="afedf-117">Application</span></span>|<span data-ttu-id="afedf-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afedf-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="afedf-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="afedf-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="afedf-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="afedf-120">Global Administrator</span></span>
* <span data-ttu-id="afedf-121">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="afedf-121">External Identity Provider Administrator</span></span>
* <span data-ttu-id="afedf-122">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="afedf-122">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="afedf-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afedf-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="afedf-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afedf-124">Request headers</span></span>

|<span data-ttu-id="afedf-125">Имя</span><span class="sxs-lookup"><span data-stu-id="afedf-125">Name</span></span>|<span data-ttu-id="afedf-126">Описание</span><span class="sxs-lookup"><span data-stu-id="afedf-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="afedf-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afedf-127">Authorization</span></span>|<span data-ttu-id="afedf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afedf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afedf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afedf-130">Request body</span></span>

<span data-ttu-id="afedf-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afedf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afedf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="afedf-132">Response</span></span>

<span data-ttu-id="afedf-133">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) и/или [builtinIdentityProvider](../resources/builtinidentityprovider.md) в тексте ответа для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="afedf-133">If successful, this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md) and/or [builtinIdentityProvider](../resources/builtinidentityprovider.md) objects in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="afedf-134">Для клиента Azure AD B2C этот метод возвращает код отклика и коллекцию `200 OK` [объектов socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) и/или [объектов appleIdentityProvider](../resources/appleidentityprovider.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="afedf-134">For an Azure AD B2C tenant this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afedf-135">Пример</span><span class="sxs-lookup"><span data-stu-id="afedf-135">Example</span></span>

### <a name="example-1-list-all-identityprovider-configured-in-an-azure-ad-tenant"></a><span data-ttu-id="afedf-136">Пример 1. Список всех **identityProvider,** настроенных в клиенте Azure AD</span><span class="sxs-lookup"><span data-stu-id="afedf-136">Example 1: List all **identityProvider** configured in an Azure AD tenant</span></span>

### <a name="request"></a><span data-ttu-id="afedf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="afedf-137">Request</span></span>
<span data-ttu-id="afedf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afedf-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="afedf-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="afedf-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="afedf-140">C#</span><span class="sxs-lookup"><span data-stu-id="afedf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afedf-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afedf-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afedf-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afedf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afedf-143">Java</span><span class="sxs-lookup"><span data-stu-id="afedf-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afedf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="afedf-144">Response</span></span>
<span data-ttu-id="afedf-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afedf-145">The following is an example of the response.</span></span>

<span data-ttu-id="afedf-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="afedf-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a><span data-ttu-id="afedf-147">Пример 2. Список всех **identityProvider,** настроенных в клиенте Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="afedf-147">Example 2: List all **identityProvider** configured in an Azure AD B2C tenant</span></span>

### <a name="request"></a><span data-ttu-id="afedf-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="afedf-148">Request</span></span>
<span data-ttu-id="afedf-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afedf-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a><span data-ttu-id="afedf-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="afedf-150">Response</span></span>
<span data-ttu-id="afedf-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afedf-151">The following is an example of the response.</span></span>

<span data-ttu-id="afedf-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="afedf-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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
