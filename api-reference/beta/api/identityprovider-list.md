---
title: Перечисление объектов identityProvider
description: Получение списка объектов identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13c6a69643b3e96fa56e7218f936fe7029d3f558
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001626"
---
# <a name="list-identityproviders"></a><span data-ttu-id="46dee-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="46dee-103">List identityProviders</span></span>

<span data-ttu-id="46dee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46dee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46dee-105">Получение списка объектов [идентитипровидерс](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="46dee-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="46dee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46dee-106">Permissions</span></span>

<span data-ttu-id="46dee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46dee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46dee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46dee-109">Permission type</span></span>      | <span data-ttu-id="46dee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46dee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46dee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46dee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46dee-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46dee-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="46dee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46dee-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="46dee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46dee-114">Not supported.</span></span>|
|<span data-ttu-id="46dee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46dee-115">Application</span></span>|<span data-ttu-id="46dee-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46dee-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="46dee-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="46dee-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="46dee-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="46dee-118">Global administrator</span></span>
* <span data-ttu-id="46dee-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="46dee-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="46dee-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46dee-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="46dee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46dee-121">Request headers</span></span>

|<span data-ttu-id="46dee-122">Имя</span><span class="sxs-lookup"><span data-stu-id="46dee-122">Name</span></span>|<span data-ttu-id="46dee-123">Описание</span><span class="sxs-lookup"><span data-stu-id="46dee-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="46dee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46dee-124">Authorization</span></span>|<span data-ttu-id="46dee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46dee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46dee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46dee-127">Request body</span></span>

<span data-ttu-id="46dee-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46dee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46dee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="46dee-129">Response</span></span>

<span data-ttu-id="46dee-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [IdentityProvider](../resources/identityprovider.md) и [Опенидконнектпровидер](../resources/openIdConnectProvider.md) (только для Azure AD B2C) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46dee-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46dee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="46dee-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="46dee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46dee-132">Request</span></span>

<span data-ttu-id="46dee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46dee-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="46dee-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="46dee-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="46dee-135">C#</span><span class="sxs-lookup"><span data-stu-id="46dee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46dee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46dee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46dee-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46dee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46dee-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="46dee-138">Response</span></span>

<span data-ttu-id="46dee-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="46dee-139">The following is an example of the response.</span></span>

<span data-ttu-id="46dee-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="46dee-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


