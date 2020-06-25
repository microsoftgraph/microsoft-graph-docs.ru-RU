---
title: Назначение типа ресурса claimsMappingPolicy
description: Назначьте Клаимсмаппингполици для servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b22afa1dd68f90bbae069055fb0999a90ed17a0b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863560"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="8f4b7-103">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8f4b7-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="8f4b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f4b7-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8f4b7-105">Назначьте [клаимсмаппингполици](../resources/claimsmappingpolicy.md) для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="8f4b7-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f4b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4b7-106">Permissions</span></span>

<span data-ttu-id="8f4b7-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8f4b7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4b7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f4b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4b7-109">Permission type</span></span>                        | <span data-ttu-id="8f4b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f4b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f4b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f4b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f4b7-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f4b7-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="8f4b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f4b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-114">Not supported.</span></span> |
| <span data-ttu-id="8f4b7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f4b7-115">Application</span></span>                            | <span data-ttu-id="8f4b7-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f4b7-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f4b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8f4b7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f4b7-118">Request headers</span></span>

| <span data-ttu-id="8f4b7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f4b7-119">Name</span></span>          | <span data-ttu-id="8f4b7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f4b7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f4b7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f4b7-121">Authorization</span></span> | <span data-ttu-id="8f4b7-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-122">Bearer {token}.</span></span> <span data-ttu-id="8f4b7-123">Required.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-123">Required.</span></span> |
| <span data-ttu-id="8f4b7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f4b7-124">Content-Type</span></span> | <span data-ttu-id="8f4b7-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-125">application/json.</span></span> <span data-ttu-id="8f4b7-126">Required.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f4b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f4b7-127">Request body</span></span>

<span data-ttu-id="8f4b7-128">В тексте запроса укажите идентификатор объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-128">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="8f4b7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4b7-129">Response</span></span>

<span data-ttu-id="8f4b7-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="8f4b7-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f4b7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f4b7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f4b7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f4b7-133">Request</span></span>

<span data-ttu-id="8f4b7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f4b7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4b7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="8f4b7-136">C#</span><span class="sxs-lookup"><span data-stu-id="8f4b7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f4b7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f4b7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f4b7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f4b7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f4b7-139">Java</span><span class="sxs-lookup"><span data-stu-id="8f4b7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f4b7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4b7-140">Response</span></span>

<span data-ttu-id="8f4b7-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f4b7-141">The following is an example of the response.</span></span>

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
  "description": "Assign claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
