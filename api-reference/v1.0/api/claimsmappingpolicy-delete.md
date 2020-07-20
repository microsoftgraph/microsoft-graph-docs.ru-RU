---
title: Удаление Клаимсмаппингполици
description: Удаление Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5749effbb234444cf3ba609df58a0af598c9b204
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863840"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="dca16-103">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="dca16-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="dca16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dca16-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dca16-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dca16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dca16-106">Permissions</span></span>

<span data-ttu-id="dca16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dca16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dca16-109">Permission type</span></span>                        | <span data-ttu-id="dca16-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dca16-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dca16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dca16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dca16-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dca16-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="dca16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dca16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca16-114">Not supported.</span></span> |
| <span data-ttu-id="dca16-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dca16-115">Application</span></span>                            | <span data-ttu-id="dca16-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dca16-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="dca16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dca16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dca16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dca16-118">Request headers</span></span>

| <span data-ttu-id="dca16-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dca16-119">Name</span></span>          | <span data-ttu-id="dca16-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dca16-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dca16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dca16-121">Authorization</span></span> | <span data-ttu-id="dca16-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="dca16-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dca16-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dca16-123">Request body</span></span>

<span data-ttu-id="dca16-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dca16-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dca16-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca16-125">Response</span></span>

<span data-ttu-id="dca16-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dca16-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dca16-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="dca16-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dca16-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="dca16-128">Request</span></span>

<span data-ttu-id="dca16-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dca16-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dca16-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dca16-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="dca16-131">C#</span><span class="sxs-lookup"><span data-stu-id="dca16-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dca16-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dca16-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dca16-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dca16-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dca16-134">Java</span><span class="sxs-lookup"><span data-stu-id="dca16-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dca16-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca16-135">Response</span></span>

<span data-ttu-id="dca16-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dca16-136">The following is an example of the response.</span></span>

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
