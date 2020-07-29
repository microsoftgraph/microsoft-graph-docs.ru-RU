---
title: Получение identityProvider
description: Получение свойств и связей объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 288c84eef3efc0ca8495b3d579a0e02607faf40d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509728"
---
# <a name="get-identityprovider"></a><span data-ttu-id="45f08-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="45f08-103">Get identityProvider</span></span>

<span data-ttu-id="45f08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45f08-105">Получение свойств и связей объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="45f08-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45f08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45f08-106">Permissions</span></span>

<span data-ttu-id="45f08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45f08-109">Permission type</span></span>      | <span data-ttu-id="45f08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45f08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45f08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45f08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45f08-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f08-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="45f08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45f08-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="45f08-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f08-114">Not supported.</span></span>|
|<span data-ttu-id="45f08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45f08-115">Application</span></span>|<span data-ttu-id="45f08-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f08-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="45f08-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="45f08-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="45f08-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="45f08-118">Global administrator</span></span>
* <span data-ttu-id="45f08-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="45f08-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="45f08-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45f08-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="45f08-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45f08-121">Request headers</span></span>

|<span data-ttu-id="45f08-122">Имя</span><span class="sxs-lookup"><span data-stu-id="45f08-122">Name</span></span>|<span data-ttu-id="45f08-123">Описание</span><span class="sxs-lookup"><span data-stu-id="45f08-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="45f08-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45f08-124">Authorization</span></span>|<span data-ttu-id="45f08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45f08-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45f08-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45f08-127">Request body</span></span>

<span data-ttu-id="45f08-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45f08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45f08-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f08-129">Response</span></span>

<span data-ttu-id="45f08-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [IdentityProvider](../resources/identityprovider.md) или [Опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45f08-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45f08-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="45f08-131">Examples</span></span>

### <a name="example-1-retrieves-a-specific-identityprovider"></a><span data-ttu-id="45f08-132">Пример 1: получение определенного объекта **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="45f08-132">Example 1: Retrieves a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="45f08-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f08-133">Request</span></span>

<span data-ttu-id="45f08-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f08-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="45f08-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f08-135">Response</span></span>

<span data-ttu-id="45f08-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="45f08-136">The following is an example of the response.</span></span>

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
### <a name="example-2-retrieves-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="45f08-137">Пример 2: получение определенного **опенидконнектпровидер** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="45f08-137">Example 2: Retrieves a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="45f08-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f08-138">Request</span></span>

<span data-ttu-id="45f08-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f08-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="45f08-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f08-140">Response</span></span>

<span data-ttu-id="45f08-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="45f08-141">The following is an example of the response.</span></span>
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
