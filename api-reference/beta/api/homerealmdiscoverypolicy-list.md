---
title: Перечисление типов ресурсов homeRealmDiscoveryPolicy
description: Получите список объектов homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: da64f9edd6f8ca39e88c3108bcb7f08ec2236b4c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435702"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="4a543-103">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="4a543-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="4a543-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a543-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a543-105">Получите список объектов [homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4a543-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a543-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a543-106">Permissions</span></span>

<span data-ttu-id="4a543-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a543-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a543-109">Permission type</span></span>                        | <span data-ttu-id="4a543-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a543-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a543-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a543-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a543-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a543-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4a543-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a543-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a543-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a543-114">Not supported.</span></span> |
| <span data-ttu-id="4a543-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a543-115">Application</span></span>                            | <span data-ttu-id="4a543-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a543-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a543-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a543-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a543-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a543-118">Optional query parameters</span></span>

<span data-ttu-id="4a543-119">Этот метод поддерживает параметры `$expand` `$filter` запроса `$select` OData и OData для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="4a543-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4a543-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4a543-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="4a543-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="4a543-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a543-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a543-122">Request headers</span></span>

| <span data-ttu-id="4a543-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4a543-123">Name</span></span>      |<span data-ttu-id="4a543-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4a543-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a543-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a543-125">Authorization</span></span> | <span data-ttu-id="4a543-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4a543-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a543-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a543-127">Request body</span></span>

<span data-ttu-id="4a543-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a543-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a543-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a543-129">Response</span></span>

<span data-ttu-id="4a543-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a543-130">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a543-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a543-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a543-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a543-132">Request</span></span>

<span data-ttu-id="4a543-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a543-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a543-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a543-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="4a543-135">C#</span><span class="sxs-lookup"><span data-stu-id="4a543-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a543-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a543-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a543-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a543-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a543-138">Java</span><span class="sxs-lookup"><span data-stu-id="4a543-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a543-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a543-139">Response</span></span>

<span data-ttu-id="4a543-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a543-140">The following is an example of the response.</span></span>

> <span data-ttu-id="4a543-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a543-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List homeRealmDiscoveryPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


