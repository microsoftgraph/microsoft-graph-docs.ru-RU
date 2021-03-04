---
title: Удаление tokenLifetimePolicy
description: Удаление tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d73fd917d7fa503857cf7592c2c95925166b133b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443393"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="8b490-103">Удаление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="8b490-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="8b490-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b490-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b490-105">Удаление [объекта tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8b490-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b490-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b490-106">Permissions</span></span>

<span data-ttu-id="8b490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b490-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b490-109">Permission type</span></span>                        | <span data-ttu-id="8b490-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b490-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b490-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b490-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b490-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b490-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8b490-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b490-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b490-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b490-114">Not supported.</span></span> |
| <span data-ttu-id="8b490-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b490-115">Application</span></span>                            | <span data-ttu-id="8b490-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b490-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b490-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b490-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b490-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b490-118">Request headers</span></span>

| <span data-ttu-id="8b490-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b490-119">Name</span></span>          | <span data-ttu-id="8b490-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8b490-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b490-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b490-121">Authorization</span></span> | <span data-ttu-id="8b490-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8b490-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b490-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b490-123">Request body</span></span>

<span data-ttu-id="8b490-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b490-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b490-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b490-125">Response</span></span>

<span data-ttu-id="8b490-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8b490-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8b490-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b490-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b490-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b490-128">Request</span></span>

<span data-ttu-id="8b490-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b490-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b490-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b490-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="8b490-131">C#</span><span class="sxs-lookup"><span data-stu-id="8b490-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b490-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b490-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b490-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b490-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b490-134">Java</span><span class="sxs-lookup"><span data-stu-id="8b490-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b490-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b490-135">Response</span></span>

<span data-ttu-id="8b490-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b490-136">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


