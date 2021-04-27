---
title: Get trustFrameworkKeySet
description: Извлечение свойств и связей объекта trustframeworkkeyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: aadc3fb05b467b91577711b29867ae0957eb8ebd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048906"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="cb160-103">Get trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="cb160-103">Get trustFrameworkKeySet</span></span>

<span data-ttu-id="cb160-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb160-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb160-105">Извлечение свойств и ассоциаций для [Trustframeworkkeyset.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="cb160-105">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb160-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb160-106">Permissions</span></span>

<span data-ttu-id="cb160-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb160-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb160-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb160-109">Permission type</span></span>                        | <span data-ttu-id="cb160-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb160-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb160-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb160-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb160-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb160-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="cb160-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb160-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb160-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb160-114">Not supported.</span></span> |
| <span data-ttu-id="cb160-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb160-115">Application</span></span>                            | <span data-ttu-id="cb160-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb160-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb160-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb160-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb160-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb160-118">Request headers</span></span>

| <span data-ttu-id="cb160-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb160-119">Name</span></span>      |<span data-ttu-id="cb160-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb160-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb160-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb160-121">Authorization</span></span> | <span data-ttu-id="cb160-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb160-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb160-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb160-124">Request body</span></span>

<span data-ttu-id="cb160-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb160-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb160-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb160-126">Response</span></span>

<span data-ttu-id="cb160-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb160-127">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb160-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb160-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb160-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb160-129">Request</span></span>

<span data-ttu-id="cb160-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb160-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb160-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb160-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="cb160-132">C#</span><span class="sxs-lookup"><span data-stu-id="cb160-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb160-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb160-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb160-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb160-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb160-135">Java</span><span class="sxs-lookup"><span data-stu-id="cb160-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb160-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb160-136">Response</span></span>

<span data-ttu-id="cb160-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb160-137">The following is an example of the response.</span></span>

> <span data-ttu-id="cb160-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb160-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


