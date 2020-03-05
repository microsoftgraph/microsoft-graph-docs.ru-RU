---
title: Назначение типа ресурса claimsMappingPolicy
description: Назначьте Клаимсмаппингполици участнику службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fea8527d6da5f9422e1d81c5f2a0a662dfcd00c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453368"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="c1c0b-103">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c0b-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="c1c0b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c1c0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c0b-105">Назначьте [клаимсмаппингполици](../resources/claimsmappingpolicy.md) для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0b-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c0b-106">Permissions</span></span>

<span data-ttu-id="c1c0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1c0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c0b-109">Permission type</span></span>                        | <span data-ttu-id="c1c0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1c0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1c0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1c0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1c0b-112">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c1c0b-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c1c0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1c0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c0b-114">Not supported.</span></span> |
| <span data-ttu-id="c1c0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1c0b-115">Application</span></span>                            | <span data-ttu-id="c1c0b-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c1c0b-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1c0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c1c0b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1c0b-118">Request headers</span></span>

| <span data-ttu-id="c1c0b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c1c0b-119">Name</span></span>          | <span data-ttu-id="c1c0b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c0b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1c0b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c0b-121">Authorization</span></span> | <span data-ttu-id="c1c0b-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c1c0b-122">Bearer {token}</span></span> |
| <span data-ttu-id="c1c0b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1c0b-123">Content-Type</span></span> | <span data-ttu-id="c1c0b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1c0b-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1c0b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1c0b-125">Request body</span></span>

<span data-ttu-id="c1c0b-126">В тексте запроса укажите идентификатор объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="c1c0b-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="c1c0b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c0b-127">Response</span></span>

<span data-ttu-id="c1c0b-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c1c0b-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1c0b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1c0b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1c0b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1c0b-131">Request</span></span>

<span data-ttu-id="c1c0b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1c0b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1c0b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c0b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c1c0b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c0b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1c0b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c0b-135">Response</span></span>

<span data-ttu-id="c1c0b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1c0b-136">The following is an example of the response.</span></span>

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
