---
title: Удаление Клаимсмаппингполици
description: Удаление Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9818874d247fc958292a91ce490172d8ff8b3296
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958093"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="a910c-103">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="a910c-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="a910c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a910c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a910c-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a910c-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a910c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a910c-106">Permissions</span></span>

<span data-ttu-id="a910c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a910c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a910c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a910c-109">Permission type</span></span>                        | <span data-ttu-id="a910c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a910c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a910c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a910c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a910c-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a910c-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a910c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a910c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a910c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a910c-114">Not supported.</span></span> |
| <span data-ttu-id="a910c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a910c-115">Application</span></span>                            | <span data-ttu-id="a910c-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a910c-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a910c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a910c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a910c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a910c-118">Request headers</span></span>

| <span data-ttu-id="a910c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a910c-119">Name</span></span>          | <span data-ttu-id="a910c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a910c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a910c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a910c-121">Authorization</span></span> | <span data-ttu-id="a910c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a910c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a910c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a910c-123">Request body</span></span>

<span data-ttu-id="a910c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a910c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a910c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a910c-125">Response</span></span>

<span data-ttu-id="a910c-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a910c-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a910c-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="a910c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a910c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a910c-128">Request</span></span>

<span data-ttu-id="a910c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a910c-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a910c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a910c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="a910c-131">C#</span><span class="sxs-lookup"><span data-stu-id="a910c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a910c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a910c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a910c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a910c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a910c-134">Java</span><span class="sxs-lookup"><span data-stu-id="a910c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a910c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a910c-135">Response</span></span>

<span data-ttu-id="a910c-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a910c-136">The following is an example of the response.</span></span>

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
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


