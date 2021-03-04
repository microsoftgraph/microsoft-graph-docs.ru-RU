---
title: Удаление accessPackageAssignmentPolicy
description: Удаление accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fa2ca4ac595beaf917a76c20d88d148ddf02516f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439753"
---
# <a name="delete-accesspackageassignmentpolicy"></a><span data-ttu-id="2e87c-103">Удаление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="2e87c-103">Delete accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="2e87c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e87c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e87c-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)удалите [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e87c-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), delete an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e87c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e87c-106">Permissions</span></span>

<span data-ttu-id="2e87c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e87c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e87c-109">Permission type</span></span>                        | <span data-ttu-id="2e87c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e87c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e87c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e87c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e87c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e87c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="2e87c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e87c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e87c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e87c-114">Not supported.</span></span> |
| <span data-ttu-id="2e87c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e87c-115">Application</span></span>                            | <span data-ttu-id="2e87c-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e87c-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e87c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e87c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e87c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e87c-118">Request headers</span></span>

| <span data-ttu-id="2e87c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e87c-119">Name</span></span>          | <span data-ttu-id="2e87c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e87c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2e87c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e87c-121">Authorization</span></span> | <span data-ttu-id="2e87c-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="2e87c-122">Bearer \{token\}.</span></span> <span data-ttu-id="2e87c-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2e87c-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e87c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e87c-124">Request body</span></span>

<span data-ttu-id="2e87c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e87c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e87c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e87c-126">Response</span></span>

<span data-ttu-id="2e87c-127">В случае успешной работы этот метод возвращает код ответа 204 Без контента.</span><span class="sxs-lookup"><span data-stu-id="2e87c-127">If successful, this method returns a 204 No Content response code.</span></span> <span data-ttu-id="2e87c-128">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2e87c-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e87c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e87c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e87c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e87c-130">Request</span></span>

<span data-ttu-id="2e87c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e87c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e87c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e87c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="2e87c-133">C#</span><span class="sxs-lookup"><span data-stu-id="2e87c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e87c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e87c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e87c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e87c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e87c-136">Java</span><span class="sxs-lookup"><span data-stu-id="2e87c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e87c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e87c-137">Response</span></span>

<span data-ttu-id="2e87c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e87c-138">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


