---
title: Списки keySets
description: Извлечение списка объектов trustframeworkkeyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dcfce35fa33255c456303b28f36e554b467ba629
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049634"
---
# <a name="list-keysets"></a><span data-ttu-id="1db00-103">Списки keySets</span><span class="sxs-lookup"><span data-stu-id="1db00-103">List keySets</span></span>

<span data-ttu-id="1db00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1db00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1db00-105">Извлечение списка [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="1db00-105">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1db00-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1db00-106">Permissions</span></span>

<span data-ttu-id="1db00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1db00-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1db00-109">Permission type</span></span>                        | <span data-ttu-id="1db00-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1db00-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1db00-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1db00-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1db00-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1db00-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="1db00-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1db00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db00-114">Not supported.</span></span> |
| <span data-ttu-id="1db00-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1db00-115">Application</span></span>                            | <span data-ttu-id="1db00-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1db00-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1db00-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1db00-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="1db00-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1db00-118">Request headers</span></span>

| <span data-ttu-id="1db00-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1db00-119">Name</span></span>      |<span data-ttu-id="1db00-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1db00-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1db00-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1db00-121">Authorization</span></span> | <span data-ttu-id="1db00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1db00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1db00-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1db00-124">Request body</span></span>

<span data-ttu-id="1db00-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1db00-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1db00-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db00-126">Response</span></span>

<span data-ttu-id="1db00-127">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1db00-127">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1db00-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1db00-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1db00-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1db00-129">Request</span></span>

<span data-ttu-id="1db00-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1db00-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1db00-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1db00-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets
```
# <a name="c"></a>[<span data-ttu-id="1db00-132">C#</span><span class="sxs-lookup"><span data-stu-id="1db00-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-keysets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1db00-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1db00-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-keysets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1db00-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1db00-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-keysets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1db00-135">Java</span><span class="sxs-lookup"><span data-stu-id="1db00-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-keysets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1db00-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db00-136">Response</span></span>

<span data-ttu-id="1db00-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1db00-137">The following is an example of the response.</span></span>

> <span data-ttu-id="1db00-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1db00-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "keys": [
        {
          "k": "k-value",
          "x5c": [
            "x5c-value"
          ],
          "x5t": "x5t-value",
          "kty": "kty-value",
          "use": "use-value",
          "exp": 99,
          "nbf": 99,
          "kid": "kid-value",
          "e": "e-value",
          "n": "n-value",
          "d": "d-value",
          "p": "p-value",
          "q": "q-value",
          "dp": "dp-value",
          "dq": "dq-value",
          "qi": "qi-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List keySets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


