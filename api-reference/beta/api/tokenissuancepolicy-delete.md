---
title: Удаление Токениссуанцеполици
description: Удаление Токениссуанцеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5a4cf4b4bb5138cf325a2fb6c5fd945ae86de2b
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591728"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="92159-103">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="92159-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="92159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92159-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92159-105">Удаление объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="92159-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92159-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92159-106">Permissions</span></span>

<span data-ttu-id="92159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92159-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92159-109">Permission type</span></span>                        | <span data-ttu-id="92159-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92159-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92159-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92159-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92159-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="92159-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="92159-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92159-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92159-114">Not supported.</span></span> |
| <span data-ttu-id="92159-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92159-115">Application</span></span>                            | <span data-ttu-id="92159-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="92159-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="92159-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92159-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92159-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92159-118">Request headers</span></span>

| <span data-ttu-id="92159-119">Имя</span><span class="sxs-lookup"><span data-stu-id="92159-119">Name</span></span>          | <span data-ttu-id="92159-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92159-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="92159-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92159-121">Authorization</span></span> | <span data-ttu-id="92159-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92159-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92159-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92159-124">Request body</span></span>

<span data-ttu-id="92159-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92159-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92159-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="92159-126">Response</span></span>

<span data-ttu-id="92159-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92159-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="92159-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="92159-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92159-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="92159-129">Request</span></span>

<span data-ttu-id="92159-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92159-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92159-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="92159-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="92159-132">C#</span><span class="sxs-lookup"><span data-stu-id="92159-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92159-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92159-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92159-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92159-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="92159-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="92159-135">Response</span></span>

<span data-ttu-id="92159-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92159-136">The following is an example of the response.</span></span>

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
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
