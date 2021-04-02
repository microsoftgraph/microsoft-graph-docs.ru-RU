---
title: Получение identityProvider
description: Извлечение свойств и связей объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: fc51780f2f5ab9a783b431d49e19136c1f5e3fef
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508626"
---
# <a name="get-identityprovider-deprecated"></a><span data-ttu-id="7df8a-103">Get identityProvider (deprecated)</span><span class="sxs-lookup"><span data-stu-id="7df8a-103">Get identityProvider (deprecated)</span></span>

<span data-ttu-id="7df8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="7df8a-105">Извлечение свойств и связей [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7df8a-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7df8a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7df8a-106">Permissions</span></span>

<span data-ttu-id="7df8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7df8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7df8a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7df8a-109">Permission type</span></span>      | <span data-ttu-id="7df8a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7df8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7df8a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7df8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7df8a-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7df8a-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7df8a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7df8a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7df8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7df8a-114">Not supported.</span></span>|
|<span data-ttu-id="7df8a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7df8a-115">Application</span></span>|<span data-ttu-id="7df8a-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7df8a-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="7df8a-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7df8a-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7df8a-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7df8a-118">Global administrator</span></span>
* <span data-ttu-id="7df8a-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="7df8a-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7df8a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7df8a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7df8a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7df8a-121">Request headers</span></span>

|<span data-ttu-id="7df8a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7df8a-122">Name</span></span>|<span data-ttu-id="7df8a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7df8a-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7df8a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7df8a-124">Authorization</span></span>|<span data-ttu-id="7df8a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7df8a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7df8a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7df8a-127">Request body</span></span>

<span data-ttu-id="7df8a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7df8a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7df8a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7df8a-129">Response</span></span>

<span data-ttu-id="7df8a-130">В случае успешной работы этот метод возвращает код ответа и представление JSON для `200 OK` [identityProvider](../resources/identityprovider.md) или [openIdConnectProvider](../resources/openidconnectprovider.md) (только для Azure AD B2C) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7df8a-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7df8a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7df8a-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="7df8a-132">Пример 1. Извлечение определенного удостоверенияProvider</span><span class="sxs-lookup"><span data-stu-id="7df8a-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="7df8a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7df8a-133">Request</span></span>

<span data-ttu-id="7df8a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7df8a-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7df8a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7df8a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="7df8a-136">C#</span><span class="sxs-lookup"><span data-stu-id="7df8a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7df8a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7df8a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7df8a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7df8a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7df8a-139">Java</span><span class="sxs-lookup"><span data-stu-id="7df8a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7df8a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7df8a-140">Response</span></span>

<span data-ttu-id="7df8a-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7df8a-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="7df8a-142">Пример 2. Извлечение определенного openIDConnectProvider (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="7df8a-142">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="7df8a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7df8a-143">Request</span></span>

<span data-ttu-id="7df8a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7df8a-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7df8a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7df8a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="7df8a-146">C#</span><span class="sxs-lookup"><span data-stu-id="7df8a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7df8a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7df8a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7df8a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7df8a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7df8a-149">Java</span><span class="sxs-lookup"><span data-stu-id="7df8a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7df8a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7df8a-150">Response</span></span>

<span data-ttu-id="7df8a-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7df8a-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
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
