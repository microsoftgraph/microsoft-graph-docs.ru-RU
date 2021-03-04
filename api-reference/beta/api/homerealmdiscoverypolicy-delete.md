---
title: Удаление homeRealmDiscoveryPolicy
description: Удаление homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d18b0f018eb23bf0513507884ede82cc6a9fd234
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435751"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="56ca5-103">Удаление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="56ca5-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="56ca5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56ca5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56ca5-105">Удаление [объекта homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56ca5-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56ca5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56ca5-106">Permissions</span></span>

<span data-ttu-id="56ca5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ca5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56ca5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56ca5-109">Permission type</span></span>                        | <span data-ttu-id="56ca5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56ca5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56ca5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56ca5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56ca5-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="56ca5-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="56ca5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56ca5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ca5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56ca5-114">Not supported.</span></span> |
| <span data-ttu-id="56ca5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="56ca5-115">Application</span></span>                            | <span data-ttu-id="56ca5-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="56ca5-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ca5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56ca5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56ca5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56ca5-118">Request headers</span></span>

| <span data-ttu-id="56ca5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="56ca5-119">Name</span></span>          | <span data-ttu-id="56ca5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="56ca5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="56ca5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56ca5-121">Authorization</span></span> | <span data-ttu-id="56ca5-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="56ca5-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="56ca5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56ca5-123">Request body</span></span>

<span data-ttu-id="56ca5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56ca5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56ca5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="56ca5-125">Response</span></span>

<span data-ttu-id="56ca5-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56ca5-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56ca5-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="56ca5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56ca5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="56ca5-128">Request</span></span>

<span data-ttu-id="56ca5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56ca5-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56ca5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="56ca5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="56ca5-131">C#</span><span class="sxs-lookup"><span data-stu-id="56ca5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56ca5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ca5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56ca5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56ca5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56ca5-134">Java</span><span class="sxs-lookup"><span data-stu-id="56ca5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56ca5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="56ca5-135">Response</span></span>

<span data-ttu-id="56ca5-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56ca5-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


