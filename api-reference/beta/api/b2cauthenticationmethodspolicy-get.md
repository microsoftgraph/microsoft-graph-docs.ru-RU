---
title: Получение b2cAuthenticationMethodsPolicy
description: Чтение свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 840d3be6471391e4c4128421dbf69da6efa6a985
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438402"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="7454c-103">Получение b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="7454c-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="7454c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7454c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7454c-105">Чтение свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7454c-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7454c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7454c-106">Permissions</span></span>

<span data-ttu-id="7454c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7454c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7454c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7454c-109">Permission type</span></span>                        | <span data-ttu-id="7454c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7454c-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="7454c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7454c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7454c-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7454c-112">Policy.Read.All</span></span>|
| <span data-ttu-id="7454c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7454c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7454c-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7454c-114">Policy.Read.All</span></span>|
| <span data-ttu-id="7454c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7454c-115">Application</span></span>                            | <span data-ttu-id="7454c-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7454c-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7454c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7454c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="7454c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7454c-118">Request headers</span></span>

| <span data-ttu-id="7454c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7454c-119">Name</span></span>      |<span data-ttu-id="7454c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7454c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7454c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7454c-121">Authorization</span></span> | <span data-ttu-id="7454c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7454c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7454c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7454c-124">Request body</span></span>

<span data-ttu-id="7454c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7454c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7454c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7454c-126">Response</span></span>

<span data-ttu-id="7454c-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и запрошенный объект [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7454c-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7454c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7454c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7454c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7454c-129">Request</span></span>

<span data-ttu-id="7454c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7454c-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7454c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7454c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="7454c-132">C#</span><span class="sxs-lookup"><span data-stu-id="7454c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7454c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7454c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7454c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7454c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7454c-135">Java</span><span class="sxs-lookup"><span data-stu-id="7454c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7454c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7454c-136">Response</span></span>

<span data-ttu-id="7454c-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7454c-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#b2cAuthenticationMethodsPolicy",
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get b2cAuthenticationMethodsPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
