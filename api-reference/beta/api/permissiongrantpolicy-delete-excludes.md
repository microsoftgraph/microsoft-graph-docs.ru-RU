---
title: Удаление permissionGrantConditionSet из исключения коллекции разрешенийGrantPolicy
description: Удаляет исключенный набор условий из политики предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 9215ee6d935f19581fbe855f50635f5dc0bd5c98
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447718"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="882da-103">Удаление permissionGrantConditionSet из исключения коллекции разрешенийGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="882da-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="882da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="882da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="882da-105">Удаляет [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) из  исключенной коллекции [permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="882da-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="882da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="882da-106">Permissions</span></span>

<span data-ttu-id="882da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="882da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="882da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="882da-109">Permission type</span></span>      | <span data-ttu-id="882da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="882da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="882da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="882da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="882da-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="882da-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="882da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="882da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="882da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="882da-114">Not supported.</span></span>    |
| <span data-ttu-id="882da-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="882da-115">Application</span></span> | <span data-ttu-id="882da-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="882da-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="882da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="882da-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="882da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="882da-118">Request headers</span></span>

| <span data-ttu-id="882da-119">Имя</span><span class="sxs-lookup"><span data-stu-id="882da-119">Name</span></span>       | <span data-ttu-id="882da-120">Тип</span><span class="sxs-lookup"><span data-stu-id="882da-120">Type</span></span> | <span data-ttu-id="882da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="882da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="882da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="882da-122">Authorization</span></span>  | <span data-ttu-id="882da-123">string</span><span class="sxs-lookup"><span data-stu-id="882da-123">string</span></span>  | <span data-ttu-id="882da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="882da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="882da-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="882da-126">Request body</span></span>

<span data-ttu-id="882da-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="882da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="882da-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="882da-128">Response</span></span>

<span data-ttu-id="882da-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="882da-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="882da-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="882da-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="882da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="882da-132">Request</span></span>

<span data-ttu-id="882da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="882da-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="882da-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="882da-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="882da-135">C#</span><span class="sxs-lookup"><span data-stu-id="882da-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="882da-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="882da-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="882da-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="882da-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="882da-138">Java</span><span class="sxs-lookup"><span data-stu-id="882da-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="882da-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="882da-139">Response</span></span>

<span data-ttu-id="882da-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="882da-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
