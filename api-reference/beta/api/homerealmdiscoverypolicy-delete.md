---
title: Удаление Хомереалмдисковериполици
description: Удаление Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddaaf11316804e66de03c37d52bdb338587cdc4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446571"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="620fc-103">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="620fc-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="620fc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="620fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="620fc-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="620fc-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="620fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="620fc-106">Permissions</span></span>

<span data-ttu-id="620fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="620fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="620fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="620fc-109">Permission type</span></span>                        | <span data-ttu-id="620fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="620fc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="620fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="620fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="620fc-112">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="620fc-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="620fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="620fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="620fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620fc-114">Not supported.</span></span> |
| <span data-ttu-id="620fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="620fc-115">Application</span></span>                            | <span data-ttu-id="620fc-116">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="620fc-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="620fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="620fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="620fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="620fc-118">Request headers</span></span>

| <span data-ttu-id="620fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="620fc-119">Name</span></span>          | <span data-ttu-id="620fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="620fc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="620fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="620fc-121">Authorization</span></span> | <span data-ttu-id="620fc-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="620fc-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="620fc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="620fc-123">Request body</span></span>

<span data-ttu-id="620fc-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="620fc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="620fc-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="620fc-125">Response</span></span>

<span data-ttu-id="620fc-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="620fc-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="620fc-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="620fc-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="620fc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="620fc-128">Request</span></span>

<span data-ttu-id="620fc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="620fc-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="620fc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="620fc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="620fc-131">C#</span><span class="sxs-lookup"><span data-stu-id="620fc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="620fc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="620fc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="620fc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="620fc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="620fc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="620fc-134">Response</span></span>

<span data-ttu-id="620fc-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="620fc-135">The following is an example of the response.</span></span>

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
