---
title: Удаление Клаимсмаппингполици
description: Удаление Клаимсмаппингполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cf08fd80528bf521ee0951a61d1d6e9caf28805
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476297"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="66255-103">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="66255-103">Delete claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66255-104">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="66255-104">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66255-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66255-105">Permissions</span></span>

<span data-ttu-id="66255-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66255-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66255-108">Permission type</span></span>                        | <span data-ttu-id="66255-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66255-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66255-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66255-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66255-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="66255-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="66255-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66255-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66255-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66255-113">Not supported.</span></span> |
| <span data-ttu-id="66255-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66255-114">Application</span></span>                            | <span data-ttu-id="66255-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="66255-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="66255-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66255-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66255-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66255-117">Request headers</span></span>

| <span data-ttu-id="66255-118">Имя</span><span class="sxs-lookup"><span data-stu-id="66255-118">Name</span></span>          | <span data-ttu-id="66255-119">Описание</span><span class="sxs-lookup"><span data-stu-id="66255-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66255-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66255-120">Authorization</span></span> | <span data-ttu-id="66255-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="66255-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="66255-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66255-122">Request body</span></span>

<span data-ttu-id="66255-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66255-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66255-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="66255-124">Response</span></span>

<span data-ttu-id="66255-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="66255-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="66255-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="66255-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66255-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="66255-127">Request</span></span>

<span data-ttu-id="66255-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66255-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="66255-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="66255-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66255-130">C#</span><span class="sxs-lookup"><span data-stu-id="66255-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66255-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66255-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66255-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66255-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66255-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="66255-133">Response</span></span>

<span data-ttu-id="66255-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="66255-134">The following is an example of the response.</span></span>

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
