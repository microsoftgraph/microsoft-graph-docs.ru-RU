---
title: Удаление Клаимсмаппингполици
description: Удаление Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ff68292b6140f3c0175f28adecacb68e18a0cc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966256"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="cffb9-103">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="cffb9-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="cffb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cffb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cffb9-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cffb9-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cffb9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cffb9-106">Permissions</span></span>

<span data-ttu-id="cffb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cffb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cffb9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cffb9-109">Permission type</span></span>                        | <span data-ttu-id="cffb9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cffb9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cffb9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cffb9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cffb9-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cffb9-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cffb9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cffb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cffb9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cffb9-114">Not supported.</span></span> |
| <span data-ttu-id="cffb9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cffb9-115">Application</span></span>                            | <span data-ttu-id="cffb9-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cffb9-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cffb9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cffb9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cffb9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cffb9-118">Request headers</span></span>

| <span data-ttu-id="cffb9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cffb9-119">Name</span></span>          | <span data-ttu-id="cffb9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cffb9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cffb9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cffb9-121">Authorization</span></span> | <span data-ttu-id="cffb9-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="cffb9-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cffb9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cffb9-123">Request body</span></span>

<span data-ttu-id="cffb9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cffb9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cffb9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="cffb9-125">Response</span></span>

<span data-ttu-id="cffb9-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cffb9-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cffb9-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="cffb9-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cffb9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="cffb9-128">Request</span></span>

<span data-ttu-id="cffb9-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cffb9-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cffb9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cffb9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="cffb9-131">C#</span><span class="sxs-lookup"><span data-stu-id="cffb9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cffb9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cffb9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cffb9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cffb9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cffb9-134">Java</span><span class="sxs-lookup"><span data-stu-id="cffb9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cffb9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cffb9-135">Response</span></span>

<span data-ttu-id="cffb9-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cffb9-136">The following is an example of the response.</span></span>

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

