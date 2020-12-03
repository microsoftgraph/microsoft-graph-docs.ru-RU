---
title: Удаление Пермиссионгранткондитионсет из коллекции исключений Пермиссионгрантполици
description: Удаляет исключенный набор условий из политики предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 745e42b4d236177febe3486ba1dfcbf427fe27bd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524400"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="30153-103">Удаление Пермиссионгранткондитионсет из коллекции исключений Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="30153-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="30153-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30153-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30153-105">Удаляет объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) из коллекции **исключений** объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30153-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="30153-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30153-106">Permissions</span></span>

<span data-ttu-id="30153-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30153-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30153-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30153-109">Permission type</span></span>      | <span data-ttu-id="30153-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30153-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="30153-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30153-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30153-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="30153-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="30153-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30153-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30153-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30153-114">Not supported.</span></span>    |
| <span data-ttu-id="30153-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="30153-115">Application</span></span> | <span data-ttu-id="30153-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="30153-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30153-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30153-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="30153-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30153-118">Request headers</span></span>

| <span data-ttu-id="30153-119">Имя</span><span class="sxs-lookup"><span data-stu-id="30153-119">Name</span></span>       | <span data-ttu-id="30153-120">Тип</span><span class="sxs-lookup"><span data-stu-id="30153-120">Type</span></span> | <span data-ttu-id="30153-121">Описание</span><span class="sxs-lookup"><span data-stu-id="30153-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="30153-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30153-122">Authorization</span></span>  | <span data-ttu-id="30153-123">string</span><span class="sxs-lookup"><span data-stu-id="30153-123">string</span></span>  | <span data-ttu-id="30153-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30153-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30153-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30153-126">Request body</span></span>

<span data-ttu-id="30153-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30153-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30153-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="30153-128">Response</span></span>

<span data-ttu-id="30153-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="30153-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30153-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="30153-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30153-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="30153-132">Request</span></span>

<span data-ttu-id="30153-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30153-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="30153-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="30153-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="30153-135">C#</span><span class="sxs-lookup"><span data-stu-id="30153-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30153-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30153-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30153-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30153-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30153-138">Java</span><span class="sxs-lookup"><span data-stu-id="30153-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30153-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="30153-139">Response</span></span>

<span data-ttu-id="30153-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="30153-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
