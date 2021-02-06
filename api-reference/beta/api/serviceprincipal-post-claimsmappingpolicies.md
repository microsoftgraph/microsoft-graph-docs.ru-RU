---
title: Назначение типа ресурса claimsMappingPolicy
description: Назначьте claimsMappingPolicy для основного службы.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8f2ba6bafa30b52036216d8faacea9865f84e6db
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134206"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="da14c-103">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="da14c-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="da14c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da14c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da14c-105">[Назначьте claimsMappingPolicy](../resources/claimsmappingpolicy.md) [servicePrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="da14c-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da14c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da14c-106">Permissions</span></span>

<span data-ttu-id="da14c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da14c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da14c-109">Permission type</span></span>                        | <span data-ttu-id="da14c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da14c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da14c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da14c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da14c-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da14c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="da14c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da14c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da14c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da14c-114">Not supported.</span></span> |
| <span data-ttu-id="da14c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da14c-115">Application</span></span>                            | <span data-ttu-id="da14c-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da14c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da14c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da14c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="da14c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da14c-118">Request headers</span></span>

| <span data-ttu-id="da14c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="da14c-119">Name</span></span>          | <span data-ttu-id="da14c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da14c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="da14c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da14c-121">Authorization</span></span> | <span data-ttu-id="da14c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="da14c-122">Bearer {token}</span></span> |
| <span data-ttu-id="da14c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da14c-123">Content-Type</span></span> | <span data-ttu-id="da14c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="da14c-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="da14c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da14c-125">Request body</span></span>

<span data-ttu-id="da14c-126">В теле запроса укавите идентификатор объекта [claimsMappingPolicy](../resources/claimsmappingpolicy.md) (используя свойство), который должен быть назначен основному `@odata.id` объекту-службе.</span><span class="sxs-lookup"><span data-stu-id="da14c-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="da14c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="da14c-127">Response</span></span>

<span data-ttu-id="da14c-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="da14c-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da14c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="da14c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da14c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="da14c-131">Request</span></span>

<span data-ttu-id="da14c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da14c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da14c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="da14c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="da14c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da14c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="da14c-135">C#</span><span class="sxs-lookup"><span data-stu-id="da14c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da14c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da14c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da14c-137">Java</span><span class="sxs-lookup"><span data-stu-id="da14c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da14c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da14c-138">Response</span></span>

<span data-ttu-id="da14c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da14c-139">The following is an example of the response.</span></span>

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



