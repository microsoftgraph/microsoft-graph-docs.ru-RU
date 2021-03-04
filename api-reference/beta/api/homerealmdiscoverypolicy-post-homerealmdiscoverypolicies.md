---
title: Создание homeRealmDiscoveryPolicy
description: Создайте новый homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ae8899bf66e8c46bd593c88fe456d43a85ad7760
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435674"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="f58cc-103">Создание homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="f58cc-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="f58cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f58cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f58cc-105">Создайте новый [объект homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f58cc-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f58cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f58cc-106">Permissions</span></span>

<span data-ttu-id="f58cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f58cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f58cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f58cc-109">Permission type</span></span>                        | <span data-ttu-id="f58cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f58cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f58cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f58cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f58cc-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f58cc-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f58cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f58cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f58cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f58cc-114">Not supported.</span></span> |
| <span data-ttu-id="f58cc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f58cc-115">Application</span></span>                            | <span data-ttu-id="f58cc-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f58cc-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f58cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f58cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f58cc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f58cc-118">Request headers</span></span>

| <span data-ttu-id="f58cc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f58cc-119">Name</span></span>          | <span data-ttu-id="f58cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f58cc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f58cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f58cc-121">Authorization</span></span> | <span data-ttu-id="f58cc-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f58cc-122">Bearer {token}</span></span> |
| <span data-ttu-id="f58cc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f58cc-123">Content-type</span></span> | <span data-ttu-id="f58cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f58cc-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f58cc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f58cc-125">Request body</span></span>

<span data-ttu-id="f58cc-126">В теле запроса поставляем JSON представление [объекта homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f58cc-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f58cc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f58cc-127">Response</span></span>

<span data-ttu-id="f58cc-128">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f58cc-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f58cc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="f58cc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f58cc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f58cc-130">Request</span></span>

<span data-ttu-id="f58cc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f58cc-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f58cc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f58cc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="f58cc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f58cc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f58cc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f58cc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f58cc-135">C#</span><span class="sxs-lookup"><span data-stu-id="f58cc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f58cc-136">Java</span><span class="sxs-lookup"><span data-stu-id="f58cc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f58cc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f58cc-137">Response</span></span>

<span data-ttu-id="f58cc-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f58cc-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f58cc-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f58cc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


