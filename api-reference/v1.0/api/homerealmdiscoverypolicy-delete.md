---
title: Удаление homeRealmDiscoveryPolicy
description: Удаление homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 803b770daa1a1e8f4aa073a83fc6214e2a862991
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434358"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="e2a18-103">Удаление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e2a18-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="e2a18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2a18-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e2a18-105">Удаление [объекта homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2a18-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a18-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2a18-106">Permissions</span></span>

<span data-ttu-id="e2a18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2a18-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2a18-109">Permission type</span></span>                        | <span data-ttu-id="e2a18-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2a18-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2a18-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2a18-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2a18-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2a18-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e2a18-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2a18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a18-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2a18-114">Not supported.</span></span> |
| <span data-ttu-id="e2a18-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2a18-115">Application</span></span>                            | <span data-ttu-id="e2a18-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2a18-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2a18-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2a18-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e2a18-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2a18-118">Request headers</span></span>

| <span data-ttu-id="e2a18-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2a18-119">Name</span></span>          | <span data-ttu-id="e2a18-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2a18-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e2a18-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2a18-121">Authorization</span></span> | <span data-ttu-id="e2a18-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2a18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a18-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2a18-124">Request body</span></span>

<span data-ttu-id="e2a18-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2a18-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2a18-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2a18-126">Response</span></span>

<span data-ttu-id="e2a18-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2a18-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e2a18-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e2a18-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2a18-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2a18-129">Request</span></span>

<span data-ttu-id="e2a18-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2a18-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e2a18-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a18-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="e2a18-132">C#</span><span class="sxs-lookup"><span data-stu-id="e2a18-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2a18-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a18-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2a18-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2a18-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2a18-135">Java</span><span class="sxs-lookup"><span data-stu-id="e2a18-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2a18-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2a18-136">Response</span></span>

<span data-ttu-id="e2a18-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e2a18-137">The following is an example of the response.</span></span>

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

