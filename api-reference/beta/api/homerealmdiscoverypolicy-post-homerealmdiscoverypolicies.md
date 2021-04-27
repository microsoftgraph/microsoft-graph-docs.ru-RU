---
title: Создание homeRealmDiscoveryPolicy
description: Создайте новый homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a46fd261bc29ff3a7fb275f4f8e0f1ab6e2df21f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040912"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="65b0e-103">Создание homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="65b0e-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="65b0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b0e-105">Создайте новый [объект homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65b0e-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65b0e-106">Permissions</span></span>

<span data-ttu-id="65b0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65b0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65b0e-109">Permission type</span></span>                        | <span data-ttu-id="65b0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65b0e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65b0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65b0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65b0e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="65b0e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="65b0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65b0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65b0e-114">Not supported.</span></span> |
| <span data-ttu-id="65b0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65b0e-115">Application</span></span>                            | <span data-ttu-id="65b0e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="65b0e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65b0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="65b0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65b0e-118">Request headers</span></span>

| <span data-ttu-id="65b0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="65b0e-119">Name</span></span>          | <span data-ttu-id="65b0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65b0e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="65b0e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b0e-121">Authorization</span></span> | <span data-ttu-id="65b0e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="65b0e-122">Bearer {token}</span></span> |
| <span data-ttu-id="65b0e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65b0e-123">Content-type</span></span> | <span data-ttu-id="65b0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65b0e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="65b0e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65b0e-125">Request body</span></span>

<span data-ttu-id="65b0e-126">В теле запроса поставляем JSON представление [объекта homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65b0e-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="65b0e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b0e-127">Response</span></span>

<span data-ttu-id="65b0e-128">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="65b0e-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65b0e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="65b0e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65b0e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="65b0e-130">Request</span></span>

<span data-ttu-id="65b0e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65b0e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65b0e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b0e-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="65b0e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b0e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b0e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b0e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="65b0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="65b0e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65b0e-136">Java</span><span class="sxs-lookup"><span data-stu-id="65b0e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65b0e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b0e-137">Response</span></span>

<span data-ttu-id="65b0e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="65b0e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="65b0e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65b0e-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


