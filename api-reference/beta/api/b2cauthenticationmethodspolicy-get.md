---
title: Получение b2cAuthenticationMethodsPolicy
description: Чтение свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a90275bc0f5e3235909263a3fd7672ddddf76746
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961288"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="42b8d-103">Получение b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="42b8d-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="42b8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42b8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42b8d-105">Чтение свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="42b8d-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42b8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42b8d-106">Permissions</span></span>

<span data-ttu-id="42b8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42b8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42b8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42b8d-109">Permission type</span></span>                        | <span data-ttu-id="42b8d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42b8d-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="42b8d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42b8d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42b8d-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="42b8d-112">Policy.Read.All</span></span>|
| <span data-ttu-id="42b8d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42b8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42b8d-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="42b8d-114">Policy.Read.All</span></span>|
| <span data-ttu-id="42b8d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42b8d-115">Application</span></span>                            | <span data-ttu-id="42b8d-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="42b8d-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42b8d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42b8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="42b8d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42b8d-118">Request headers</span></span>

| <span data-ttu-id="42b8d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="42b8d-119">Name</span></span>      |<span data-ttu-id="42b8d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="42b8d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42b8d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42b8d-121">Authorization</span></span> | <span data-ttu-id="42b8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42b8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42b8d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42b8d-124">Request body</span></span>

<span data-ttu-id="42b8d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42b8d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42b8d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="42b8d-126">Response</span></span>

<span data-ttu-id="42b8d-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и запрошенный объект [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42b8d-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42b8d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="42b8d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42b8d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="42b8d-129">Request</span></span>

<span data-ttu-id="42b8d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42b8d-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="42b8d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="42b8d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="42b8d-132">C#</span><span class="sxs-lookup"><span data-stu-id="42b8d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42b8d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42b8d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42b8d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42b8d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42b8d-135">Java</span><span class="sxs-lookup"><span data-stu-id="42b8d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42b8d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="42b8d-136">Response</span></span>

<span data-ttu-id="42b8d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42b8d-137">The following is an example of the response.</span></span>

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
