---
title: Получение identityProvider
description: Извлечение свойств и связей объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 31ae4f9ffad6f85466af0adede65c683499e06bd
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921518"
---
# <a name="get-identityprovider"></a><span data-ttu-id="d651c-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="d651c-103">Get identityProvider</span></span>

<span data-ttu-id="d651c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d651c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d651c-105">Извлечение свойств и связей [socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d651c-105">Retrieve the properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in Azure AD.</span></span>

<span data-ttu-id="d651c-106">Для Azure AD B2C он может получать свойства и связи [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="d651c-106">For Azure AD B2C, it can retrieve properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d651c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d651c-107">Permissions</span></span>

<span data-ttu-id="d651c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d651c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d651c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d651c-110">Permission type</span></span>      | <span data-ttu-id="d651c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d651c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d651c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d651c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d651c-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d651c-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d651c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d651c-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d651c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d651c-115">Not supported.</span></span>|
|<span data-ttu-id="d651c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d651c-116">Application</span></span>|<span data-ttu-id="d651c-117">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d651c-117">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="d651c-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d651c-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d651c-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d651c-119">Global Administrator</span></span>
* <span data-ttu-id="d651c-120">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="d651c-120">External Identity Provider Administrator</span></span>
* <span data-ttu-id="d651c-121">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="d651c-121">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d651c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d651c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d651c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d651c-123">Request headers</span></span>

|<span data-ttu-id="d651c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d651c-124">Name</span></span>|<span data-ttu-id="d651c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d651c-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d651c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d651c-126">Authorization</span></span>|<span data-ttu-id="d651c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d651c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d651c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d651c-129">Request body</span></span>

<span data-ttu-id="d651c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d651c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d651c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d651c-131">Response</span></span>

<span data-ttu-id="d651c-132">В случае успеха этот метод возвращает код отклика и представление JSON для `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md) в тексте ответа для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d651c-132">If successful, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="d651c-133">Для клиента Azure AD B2C этот метод возвращает код отклика и представление JSON для `200 OK` [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider](../resources/appleidentityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d651c-133">For an Azure AD B2C tenant, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d651c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="d651c-134">Examples</span></span>

### <a name="example-1-retrieve-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="d651c-135">Пример 1. Извлечение определенного **поставщика социальных удостоверений** (Azure AD или Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d651c-135">Example 1: Retrieve a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d651c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d651c-136">Request</span></span>

<span data-ttu-id="d651c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d651c-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d651c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d651c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
```
# <a name="c"></a>[<span data-ttu-id="d651c-139">C#</span><span class="sxs-lookup"><span data-stu-id="d651c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d651c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d651c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d651c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d651c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d651c-142">Java</span><span class="sxs-lookup"><span data-stu-id="d651c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d651c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d651c-143">Response</span></span>

<span data-ttu-id="d651c-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d651c-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "displayName": "Amazon",
    "identityProviderType": "Amazon",
    "clientId": "09876545678908765978678",
    "clientSecret": "******"
}
```

### <a name="example-2-retrieve-a-specific-built-in-identity-provider-only-for-azure-ad"></a><span data-ttu-id="d651c-145">Пример 2. Извлечение определенного встроенного поставщика **удостоверений** (только для Azure AD)</span><span class="sxs-lookup"><span data-stu-id="d651c-145">Example 2: Retrieve a specific **built-in identity provider** (only for Azure AD)</span></span>

#### <a name="request"></a><span data-ttu-id="d651c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d651c-146">Request</span></span>

<span data-ttu-id="d651c-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d651c-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d651c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d651c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_builtinidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/MSASignup-OAUTH
```
# <a name="c"></a>[<span data-ttu-id="d651c-149">C#</span><span class="sxs-lookup"><span data-stu-id="d651c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-builtinidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d651c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d651c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-builtinidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d651c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d651c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-builtinidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d651c-152">Java</span><span class="sxs-lookup"><span data-stu-id="d651c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-builtinidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d651c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d651c-153">Response</span></span>

<span data-ttu-id="d651c-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d651c-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "MSASignup-OAUTH",
    "identityProviderType": "MicrosoftAccount",
    "displayName": "MicrosoftAccount"
}
```

### <a name="example-3-retrieve-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="d651c-155">Пример 3. Извлечение определенного **поставщика удостоверений OpenID Connect** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d651c-155">Example 3: Retrieve a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d651c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d651c-156">Request</span></span>

<span data-ttu-id="d651c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d651c-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d651c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d651c-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000
```
# <a name="c"></a>[<span data-ttu-id="d651c-159">C#</span><span class="sxs-lookup"><span data-stu-id="d651c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d651c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d651c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d651c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d651c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d651c-162">Java</span><span class="sxs-lookup"><span data-stu-id="d651c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d651c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d651c-163">Response</span></span>

<span data-ttu-id="d651c-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d651c-164">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000",
  "displayName": "Login with the Contoso identity provider",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```

### <a name="example-4-retrieves-apple-identity-provideronly-for-azure-ad-b2c"></a><span data-ttu-id="d651c-165">Пример 4. Извлечение поставщика удостоверений Apple (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d651c-165">Example 4: Retrieves Apple identity provider(only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d651c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="d651c-166">Request</span></span>

<span data-ttu-id="d651c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d651c-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d651c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="d651c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
```
# <a name="c"></a>[<span data-ttu-id="d651c-169">C#</span><span class="sxs-lookup"><span data-stu-id="d651c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applemanagedidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d651c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d651c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applemanagedidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d651c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d651c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applemanagedidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d651c-172">Java</span><span class="sxs-lookup"><span data-stu-id="d651c-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applemanagedidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d651c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="d651c-173">Response</span></span>

<span data-ttu-id="d651c-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d651c-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Apple-Managed-OIDC",
    "displayName": "Sign in with Apple",
    "developerId": "UBF8T346G9",
    "serviceId": "com.microsoft.rts.b2c.test.client",
    "keyId": "99P6D879C4",
    "certificateData": "******"
}
```
