---
title: Удаление delegatedPermissionClassification
description: Удаление делегированной классификации разрешений из директора-службы API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: aa10fbf12e0fef1ef6b8a96ec61cbb0571d47f8b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137405"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="a3323-103">Удаление delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="a3323-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="a3323-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3323-105">Удаляет [delegatedPermissionClassification,](../resources/delegatedPermissionClassification.md) который ранее был настроен для делегирования разрешения.</span><span class="sxs-lookup"><span data-stu-id="a3323-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3323-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3323-106">Permissions</span></span>

<span data-ttu-id="a3323-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3323-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3323-109">Permission type</span></span>      | <span data-ttu-id="a3323-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3323-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3323-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3323-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3323-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="a3323-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3323-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3323-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3323-114">Not supported.</span></span>    |
|<span data-ttu-id="a3323-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3323-115">Application</span></span> | <span data-ttu-id="a3323-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3323-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3323-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a3323-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3323-118">Request headers</span></span>

| <span data-ttu-id="a3323-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a3323-119">Name</span></span>       | <span data-ttu-id="a3323-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a3323-120">Type</span></span> | <span data-ttu-id="a3323-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a3323-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3323-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3323-122">Authorization</span></span>  | <span data-ttu-id="a3323-123">string</span><span class="sxs-lookup"><span data-stu-id="a3323-123">string</span></span>  | <span data-ttu-id="a3323-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3323-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3323-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3323-126">Request body</span></span>

<span data-ttu-id="a3323-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3323-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3323-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3323-128">Response</span></span>

<span data-ttu-id="a3323-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a3323-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3323-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3323-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3323-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3323-132">Request</span></span>

<span data-ttu-id="a3323-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3323-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3323-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="a3323-135">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-138">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-delegatedpermissionclassifications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3323-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3323-139">Response</span></span>

<span data-ttu-id="a3323-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a3323-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

