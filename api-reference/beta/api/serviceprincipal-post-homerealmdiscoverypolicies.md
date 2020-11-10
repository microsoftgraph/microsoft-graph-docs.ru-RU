---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте Хомереалмдисковериполици участнику службы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eecb6ddb41e7f64788e8fea83be4ac18b9771421
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979648"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="005ac-103">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="005ac-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="005ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="005ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="005ac-105">Назначьте [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="005ac-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="005ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="005ac-106">Permissions</span></span>

<span data-ttu-id="005ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="005ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="005ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="005ac-109">Permission type</span></span>                        | <span data-ttu-id="005ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="005ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="005ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="005ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="005ac-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="005ac-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="005ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="005ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="005ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="005ac-114">Not supported.</span></span> |
| <span data-ttu-id="005ac-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="005ac-115">Application</span></span>                            | <span data-ttu-id="005ac-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="005ac-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="005ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="005ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="005ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="005ac-118">Request headers</span></span>

| <span data-ttu-id="005ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="005ac-119">Name</span></span>          | <span data-ttu-id="005ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="005ac-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="005ac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="005ac-121">Authorization</span></span> | <span data-ttu-id="005ac-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="005ac-122">Bearer {token}</span></span> |
| <span data-ttu-id="005ac-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="005ac-123">Content-Type</span></span> | <span data-ttu-id="005ac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="005ac-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="005ac-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="005ac-125">Request body</span></span>

<span data-ttu-id="005ac-126">В тексте запроса укажите идентификатор объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="005ac-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="005ac-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="005ac-127">Response</span></span>

<span data-ttu-id="005ac-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="005ac-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="005ac-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="005ac-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="005ac-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="005ac-131">Request</span></span>

<span data-ttu-id="005ac-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="005ac-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="005ac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="005ac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="005ac-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="005ac-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="005ac-135">C#</span><span class="sxs-lookup"><span data-stu-id="005ac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="005ac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="005ac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="005ac-137">Java</span><span class="sxs-lookup"><span data-stu-id="005ac-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="005ac-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="005ac-138">Response</span></span>

<span data-ttu-id="005ac-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="005ac-139">The following is an example of the response.</span></span>

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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


