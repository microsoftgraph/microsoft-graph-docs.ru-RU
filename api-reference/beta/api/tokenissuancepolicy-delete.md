---
title: Удаление Токениссуанцеполици
description: Удаление Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b74a0bf73db307833af871170089cb222b4b6bd
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917472"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="6dd14-103">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="6dd14-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="6dd14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd14-105">Удаление объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6dd14-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd14-106">Permissions</span></span>

<span data-ttu-id="6dd14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dd14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd14-109">Permission type</span></span>                        | <span data-ttu-id="6dd14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dd14-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6dd14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dd14-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6dd14-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6dd14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dd14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd14-114">Not supported.</span></span> |
| <span data-ttu-id="6dd14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dd14-115">Application</span></span>                            | <span data-ttu-id="6dd14-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6dd14-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dd14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6dd14-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dd14-118">Request headers</span></span>

| <span data-ttu-id="6dd14-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6dd14-119">Name</span></span>          | <span data-ttu-id="6dd14-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd14-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6dd14-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dd14-121">Authorization</span></span> | <span data-ttu-id="6dd14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dd14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dd14-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6dd14-124">Request body</span></span>

<span data-ttu-id="6dd14-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dd14-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dd14-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dd14-126">Response</span></span>

<span data-ttu-id="6dd14-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6dd14-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6dd14-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dd14-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dd14-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd14-129">Request</span></span>

<span data-ttu-id="6dd14-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dd14-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6dd14-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dd14-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="6dd14-132">C#</span><span class="sxs-lookup"><span data-stu-id="6dd14-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dd14-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dd14-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dd14-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dd14-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6dd14-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd14-135">Response</span></span>

<span data-ttu-id="6dd14-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6dd14-136">The following is an example of the response.</span></span>

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
