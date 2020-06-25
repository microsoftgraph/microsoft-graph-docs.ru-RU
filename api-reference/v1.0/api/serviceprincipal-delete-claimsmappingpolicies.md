---
title: Удаление типа ресурса claimsMappingPolicy
description: Удаление объекта Клаимсмаппингполици из servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4231bf11e28b3514f8543c41b76d132029fb122a
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864176"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="5587c-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5587c-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="5587c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5587c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5587c-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) из [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5587c-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5587c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5587c-106">Permissions</span></span>

<span data-ttu-id="5587c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5587c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5587c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5587c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5587c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5587c-109">Permission type</span></span>                        | <span data-ttu-id="5587c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5587c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5587c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5587c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5587c-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5587c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="5587c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5587c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5587c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5587c-114">Not supported.</span></span> |
| <span data-ttu-id="5587c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5587c-115">Application</span></span>                            | <span data-ttu-id="5587c-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5587c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5587c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5587c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5587c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5587c-118">Request headers</span></span>

| <span data-ttu-id="5587c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5587c-119">Name</span></span>          | <span data-ttu-id="5587c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5587c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5587c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5587c-121">Authorization</span></span> | <span data-ttu-id="5587c-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5587c-122">Bearer {token}.</span></span> <span data-ttu-id="5587c-123">Required.</span><span class="sxs-lookup"><span data-stu-id="5587c-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5587c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5587c-124">Request body</span></span>

<span data-ttu-id="5587c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5587c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5587c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5587c-126">Response</span></span>

<span data-ttu-id="5587c-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5587c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5587c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5587c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5587c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5587c-129">Request</span></span>

<span data-ttu-id="5587c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5587c-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5587c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5587c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="5587c-132">C#</span><span class="sxs-lookup"><span data-stu-id="5587c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5587c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5587c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5587c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5587c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5587c-135">Java</span><span class="sxs-lookup"><span data-stu-id="5587c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5587c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5587c-136">Response</span></span>

<span data-ttu-id="5587c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5587c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="5587c-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5587c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5587c-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5587c-139">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
