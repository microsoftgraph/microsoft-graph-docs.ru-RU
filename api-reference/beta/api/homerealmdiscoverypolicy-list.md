---
title: Перечисление типов ресурсов homeRealmDiscoveryPolicy
description: Получите список объектов homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e11c38f977562e76eb2b4805603a548730bf0ed1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040954"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="f5d40-103">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="f5d40-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="f5d40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5d40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5d40-105">Получите список объектов [homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5d40-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d40-106">Permissions</span></span>

<span data-ttu-id="f5d40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5d40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5d40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d40-109">Permission type</span></span>                        | <span data-ttu-id="f5d40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5d40-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5d40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5d40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5d40-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5d40-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f5d40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5d40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5d40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d40-114">Not supported.</span></span> |
| <span data-ttu-id="f5d40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5d40-115">Application</span></span>                            | <span data-ttu-id="f5d40-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5d40-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5d40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5d40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5d40-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5d40-118">Optional query parameters</span></span>

<span data-ttu-id="f5d40-119">Этот метод поддерживает параметры `$expand` `$filter` запроса `$select` OData и OData для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="f5d40-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f5d40-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f5d40-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="f5d40-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="f5d40-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5d40-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5d40-122">Request headers</span></span>

| <span data-ttu-id="f5d40-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f5d40-123">Name</span></span>      |<span data-ttu-id="f5d40-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f5d40-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5d40-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5d40-125">Authorization</span></span> | <span data-ttu-id="f5d40-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f5d40-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5d40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5d40-127">Request body</span></span>

<span data-ttu-id="f5d40-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5d40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5d40-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d40-129">Response</span></span>

<span data-ttu-id="f5d40-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f5d40-130">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5d40-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f5d40-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5d40-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5d40-132">Request</span></span>

<span data-ttu-id="f5d40-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5d40-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5d40-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5d40-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="f5d40-135">C#</span><span class="sxs-lookup"><span data-stu-id="f5d40-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5d40-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5d40-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5d40-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5d40-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5d40-138">Java</span><span class="sxs-lookup"><span data-stu-id="f5d40-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5d40-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d40-139">Response</span></span>

<span data-ttu-id="f5d40-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5d40-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f5d40-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f5d40-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


