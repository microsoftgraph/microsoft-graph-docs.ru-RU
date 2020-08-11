---
title: Получение identityProvider
description: Получение свойств и связей объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c7ba30513b6de77628aad6790a2050ff4ca8afb
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630279"
---
# <a name="get-identityprovider"></a><span data-ttu-id="dff34-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="dff34-103">Get identityProvider</span></span>

<span data-ttu-id="dff34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dff34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dff34-105">Получение свойств и связей объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="dff34-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dff34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dff34-106">Permissions</span></span>

<span data-ttu-id="dff34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dff34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dff34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dff34-109">Permission type</span></span>      | <span data-ttu-id="dff34-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dff34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dff34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dff34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dff34-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dff34-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="dff34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dff34-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dff34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dff34-114">Not supported.</span></span>|
|<span data-ttu-id="dff34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dff34-115">Application</span></span>|<span data-ttu-id="dff34-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dff34-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="dff34-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="dff34-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="dff34-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="dff34-118">Global administrator</span></span>
* <span data-ttu-id="dff34-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="dff34-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="dff34-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dff34-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dff34-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dff34-121">Request headers</span></span>

|<span data-ttu-id="dff34-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dff34-122">Name</span></span>|<span data-ttu-id="dff34-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dff34-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="dff34-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dff34-124">Authorization</span></span>|<span data-ttu-id="dff34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dff34-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dff34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dff34-127">Request body</span></span>

<span data-ttu-id="dff34-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dff34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dff34-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dff34-129">Response</span></span>

<span data-ttu-id="dff34-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [IdentityProvider](../resources/identityprovider.md) или [Опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dff34-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dff34-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="dff34-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="dff34-132">Пример 1: получение определенного identityProvider</span><span class="sxs-lookup"><span data-stu-id="dff34-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="dff34-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dff34-133">Request</span></span>

<span data-ttu-id="dff34-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dff34-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dff34-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dff34-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="dff34-136">C#</span><span class="sxs-lookup"><span data-stu-id="dff34-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dff34-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dff34-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dff34-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dff34-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dff34-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dff34-139">Response</span></span>

<span data-ttu-id="dff34-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dff34-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
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
### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="dff34-141">Пример 2: получение определенного Опенидконнектпровидер (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="dff34-141">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="dff34-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dff34-142">Request</span></span>

<span data-ttu-id="dff34-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dff34-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="dff34-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dff34-144">Response</span></span>

<span data-ttu-id="dff34-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dff34-145">The following is an example of the response.</span></span>
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
