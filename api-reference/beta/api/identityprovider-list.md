---
title: Перечисление объектов identityProvider
description: Извлечение списка объектов identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2b988fa0aab5e59e165defc9f953cc267606dd84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961000"
---
# <a name="list-identityproviders"></a><span data-ttu-id="beb8b-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="beb8b-103">List identityProviders</span></span>

<span data-ttu-id="beb8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb8b-105">Извлечение списка [объектов identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="beb8b-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="beb8b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beb8b-106">Permissions</span></span>

<span data-ttu-id="beb8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb8b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beb8b-109">Permission type</span></span>      | <span data-ttu-id="beb8b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beb8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beb8b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beb8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="beb8b-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb8b-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="beb8b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beb8b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="beb8b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb8b-114">Not supported.</span></span>|
|<span data-ttu-id="beb8b-115">Application</span><span class="sxs-lookup"><span data-stu-id="beb8b-115">Application</span></span>|<span data-ttu-id="beb8b-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb8b-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="beb8b-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="beb8b-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="beb8b-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="beb8b-118">Global administrator</span></span>
* <span data-ttu-id="beb8b-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="beb8b-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="beb8b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beb8b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="beb8b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beb8b-121">Request headers</span></span>

|<span data-ttu-id="beb8b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="beb8b-122">Name</span></span>|<span data-ttu-id="beb8b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="beb8b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="beb8b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beb8b-124">Authorization</span></span>|<span data-ttu-id="beb8b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb8b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb8b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beb8b-127">Request body</span></span>

<span data-ttu-id="beb8b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="beb8b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beb8b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb8b-129">Response</span></span>

<span data-ttu-id="beb8b-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов identityProvider](../resources/identityprovider.md) и [openIdConnectProvider](../resources/openIdConnectProvider.md) (только для объектов Azure AD B2C) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="beb8b-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb8b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="beb8b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb8b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="beb8b-132">Request</span></span>

<span data-ttu-id="beb8b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beb8b-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="beb8b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="beb8b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="beb8b-135">C#</span><span class="sxs-lookup"><span data-stu-id="beb8b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beb8b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beb8b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beb8b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beb8b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="beb8b-138">Java</span><span class="sxs-lookup"><span data-stu-id="beb8b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="beb8b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb8b-139">Response</span></span>

<span data-ttu-id="beb8b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="beb8b-140">The following is an example of the response.</span></span>

<span data-ttu-id="beb8b-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="beb8b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityProviders",
    "value": [
      {
          "@odata.type": "microsoft.graph.identityProvider",
          "id": "Amazon-OAUTH",
          "name": "Login with Amazon",
          "type": "Amazon",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****"
      },
      {
          "@odata.type": "microsoft.graph.openIdConnectProvider",
          "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
          "name": "Login with the Contoso identity provider",
          "type": "OpenIDConnect",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****",
          "claimsMapping": {
              "userId": "myUserId",
              "givenName": "myGivenName",
              "surname": "mySurname",
              "email": "myEmail",
              "displayName": "myDisplayName"
          },
          "domainHint": "contoso",
          "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
          "responseMode": "form_post",
          "responseType": "code",
          "scope": "openid"
      },
    ]
}
```


