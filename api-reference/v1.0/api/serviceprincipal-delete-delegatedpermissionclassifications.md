---
title: Удаление delegatedPermissionClassification
description: Удаление делегированной классификации разрешений из директора-службы API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: decce0d0a9e3f6915676cb7151da0d43ddff3067
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133100"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="9a510-103">Удаление delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="9a510-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="9a510-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a510-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a510-105">Удаляет [делегированную классификацию,](../resources/delegatedPermissionClassification.md) которая ранее была настроена для делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="9a510-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a510-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a510-106">Permissions</span></span>

<span data-ttu-id="9a510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a510-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a510-109">Permission type</span></span>      | <span data-ttu-id="9a510-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a510-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a510-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a510-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a510-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a510-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="9a510-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a510-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a510-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a510-114">Not supported.</span></span>    |
|<span data-ttu-id="9a510-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a510-115">Application</span></span> | <span data-ttu-id="9a510-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a510-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a510-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a510-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a510-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a510-118">Request headers</span></span>

| <span data-ttu-id="9a510-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9a510-119">Name</span></span>       | <span data-ttu-id="9a510-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9a510-120">Type</span></span> | <span data-ttu-id="9a510-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9a510-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a510-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a510-122">Authorization</span></span>  | <span data-ttu-id="9a510-123">string</span><span class="sxs-lookup"><span data-stu-id="9a510-123">string</span></span>  | <span data-ttu-id="9a510-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a510-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a510-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a510-126">Request body</span></span>

<span data-ttu-id="9a510-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a510-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a510-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a510-128">Response</span></span>

<span data-ttu-id="9a510-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a510-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a510-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a510-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a510-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a510-132">Request</span></span>

<span data-ttu-id="9a510-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a510-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a510-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a510-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a510-135">C#</span><span class="sxs-lookup"><span data-stu-id="9a510-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a510-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a510-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a510-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a510-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a510-138">Java</span><span class="sxs-lookup"><span data-stu-id="9a510-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-delegatedpermissionclassifications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a510-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a510-139">Response</span></span>

<span data-ttu-id="9a510-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9a510-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
